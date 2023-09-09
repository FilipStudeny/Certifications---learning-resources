# Address Resolution - ARP
Address Resolution Protocol, or ARP, is what needed to map IPv4 addresses to MAC addresses.

Every IP device on an Ethernet network has a unique Ethernet MAC address. When a device sends an Ethernet Layer 2 frame, it contains these two addresses:

- **Destination MAC address** - The Ethernet MAC address of the destination device on the same local network segment. If the destination host is on another network, then the destination address in the frame would be that of the default gateway (i.e., router).
- **Source MAC address** - The MAC address of the Ethernet NIC on the source host.

A device uses Address Resolution Protocol (ARP) to determine the destination MAC address of a local device when it knows its IPv4 address.

ARP provides two basic functions:
- Resolving IPv4 addresses to MAC addresses
- Maintaining a table of IPv4 to MAC address mappings

## ARP Functions 
When a packet is sent to the data link layer to be encapsulated into an Ethernet frame, the device refers to a table in its memory to find the MAC address that is mapped to the IPv4 address. This table is stored temporarily in RAM memory and called the ARP table or the ARP cache.

The sending device will search its ARP table for a destination IPv4 address and a corresponding MAC address.

- If the packet’s destination IPv4 address is on the same network as the source IPv4 address, the device will search the ARP table for the destination IPv4 address.
- If the destination IPv4 address is on a different network than the source IPv4 address, the device will search the ARP table for the IPv4 address of the default gateway.

In both cases, the search is for an IPv4 address and a corresponding MAC address for the device.

## ARP Request 
An ARP request is sent when a device needs to determine the MAC address that is associated with an IPv4 address, and it does not have an entry for the IPv4 address in its ARP table.

ARP messages are encapsulated directly within an Ethernet frame. There is no IPv4 header. The ARP request is encapsulated in an Ethernet frame using the following header information:

- **Destination MAC address** – This is a broadcast address FF-FF-FF-FF-FF-FF requiring all Ethernet NICs on the LAN to accept and process the ARP request.
- **Source MAC address** – This is MAC address of the sender of the ARP request.
- **Type** - ARP messages have a type field of 0x806. This informs the receiving NIC that the data portion of the frame needs to be passed to the ARP process.

Because ARP requests are broadcasts, they are flooded out all ports by the switch, except the receiving port.

## ARP Reply 
Only the device with the target IPv4 address associated with the ARP request will respond with an ARP reply. The ARP reply is encapsulated in an Ethernet frame using the following header information:

- **Destination MAC address** – This is the MAC address of the sender of the ARP request.
- **Source MAC address** – This is the MAC address of the sender of the ARP reply.
- **Type** - ARP messages have a type field of 0x806. This informs the receiving NIC that the data portion of the frame needs to be passed to the ARP process.

Only the device that originally sent the ARP request will receive the unicast ARP reply. After the ARP reply is received, the device will add the IPv4 address and the corresponding MAC address to its ARP table. Packets destined for that IPv4 address can now be encapsulated in frames using its corresponding MAC address.

If no device responds to the ARP request, the packet is dropped because a frame cannot be created.

Entries in the ARP table are time stamped. If a device does not receive a frame from a device before the timestamp expires, the entry for this device is removed from the ARP table.

> Static map entries can be entered in an ARP table, but this is rarely done. Static ARP table entries do not expire over time and must be manually removed.

> Note: IPv6 uses a similar process to ARP for IPv4, known as ICMPv6 Neighbor Discovery (ND). IPv6 uses neighbor solicitation and neighbor advertisement messages, similar to IPv4 ARP requests and ARP replies.

## ARP Role in Remote Communications 
When the destination IPv4 address is not on the same network as the source IPv4 address, the source device needs to send the frame to its default gateway. This is the interface of the local router. Whenever a source device has a packet with an IPv4 address on another network, it will encapsulate that packet in a frame using the destination MAC address of the router.

The IPv4 address of the default gateway is stored in the IPv4 configuration of the hosts. When a host creates a packet for a destination, it compares the destination IPv4 address and its own IPv4 address to determine if the two IPv4 addresses are located on the same Layer 3 network. If the destination host is not on its same network, the source checks its ARP table for an entry with the IPv4 address of the default gateway. If there is not an entry, it uses the ARP process to determine a MAC address of the default gateway.

## Removing Entries from an ARP Table 
For each device, an ARP cache timer removes ARP entries that have not been used for a specified period of time.

##  ARP Tables on Devices 

### Cisco router


    R1# show ip arp
    Protocol   Address           Age (min)  Hardware Addr   Type  Interface
    Internet   192.168.10.1            -    a0e0.af0d.e140  ARPA  GigabitEthernet0/0/0
    Internet   209.165.200.225         -    a0e0.af0d.e141  ARPA  GigabitEthernet0/0/1
    Internet   209.165.200.226         1    a03d.6fe1.9d91  ARPA  GigabitEthernet0/0/1
    R1#

### Windows 10 / Linux
    C:∖Users∖PC> arp -a
    Interface: 192.168.1.124 --- 0x10
    Internet Address     Physical Address     Type
    192.168.1.1          c8-d7-19-cc-a0-86    dynamic
    192.168.1.146        94-57-a5-0c-5b-02    dynamic
    192.168.1.255        ff-ff-ff-ff-ff-ff    static
    224.0.0.22           01-00-5e-00-00-16    static
    224.0.0.251          01-00-5e-00-00-fb    static
    ...

## ARP Issues - ARP Broadcasts and ARP Spoofing 

### ARP Broadcasts
As a broadcast frame, an ARP request is received and processed by every device on the local network. If a large number of devices were to be powered up and all start accessing network services at the same time, there could be some reduction in performance for a short period of time. In some cases, the use of ARP can lead to a potential security risk. 

### ARP Spoofing 
The threat actor sends an ARP reply with its own MAC address. The receiver of the ARP reply will add the wrong MAC address to its ARP table and send these packets to the threat actor.
Enterprise level switches include mitigation techniques known as **dynamic ARP inspection (DAI)**.