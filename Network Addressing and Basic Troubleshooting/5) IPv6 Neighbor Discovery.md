# IPv6 Neighbor Discovery
If your network is using the IPv6 communications protocol, the neighbor discovery protocol, or ND, is what you need to match IPv6 addresses to MAC addresses.

## IPv6 Neighbor Discovery Messages 
IPv6 neighbor discovery protocol is sometimes referred to as ND or NDP.

ND provides address resolution, router discovery, and redirection services for **IPv6 using ICMPv6**. **ICMPv6 ND** uses five **ICMPv6 messages** to perform these services:

- Neighbor solicitation messages
- Neighbor advertisement messages
- Router solicitation messages
- Router advertisement messages
- Redirect message

**Neighbor solicitation** and **neighbor advertisement** messages are used for device-to-device messaging such as address resolution (similar to ARP for IPv4). Devices include both host computers and routers.

**Router solicitation** and **router advertisement** messages are for messaging between devices and routers. Typically router discovery is used for dynamic address allocation and stateless address autoconfiguration (SLAAC).

## IPv6 Neighbor Discovery - Address Resolution 
IPv6 devices use IPv6 ND to determine the MAC address of a device that has a a known IPv6 address.

ICMPv6 **neighbor solicitation** and **neighbor advertisement** messages are used for MAC address resolution. This is similar to ARP Requests and ARP Replies used by ARP for IPv4. 

ICMPv6 neighbor solicitation messages are sent using special Ethernet and IPv6 multicast addresses. This allows the Ethernet NIC of the receiving device to determine whether the neighbor solicitation message is for itself without having to send it to the operating system for processing.

PC2 replies to the request with an ICMPv6 neighbor advertisement message which includes its MAC address.
