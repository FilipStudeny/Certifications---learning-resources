# Troubleshoot Common Network Problems
The following categories are used to classify types of personal data:

- **Volunteered dat**a - This is created and explicitly shared by individuals, such as social network profiles. This type of data might include video files, pictures, text, or audio files.
- **Observed data** - This is captured by recording the actions of individuals, such as location data when using cell phones.
- **Inferred data** - This is data such as a credit score, which is based on analysis of volunteered or observed data. 
    
## Network Troubleshooting Overview 
Troubleshooting is the process of identifying, locating and correcting problems. 

When troubleshooting, proper documentation must be maintained. This documentation should include as much information as possible about the following:

- The problem encountered
- Steps taken to determine the cause of the problem
- Steps to correct the problem and ensure that it will not reoccur

Document all steps taken in troubleshooting, even the ones that did not solve the issue.

## Gathering Information 
The following checklist provides some of the important information that should be checked.

**Nature of problem**

    End-user reports
    Problem verification report

**Equipment**

    Manufacturer
    Make / model
    Firmware version
    Operating system version
    Ownership / warranty information

**Configuration and Topology**

    Physical and logical topology
    Configuration files
    Log files

**Previous Troubleshooting**

    Steps taken
    Results achieved

## Structured Troubleshooting Methods 

### **Bottom-Up**
Start with the physical layer and the physical components of the network as shown in the figure, and move up through the layers of the OSI model until the cause of the problem is identified.

Bottom-up troubleshooting is a good approach to use when the problem is suspected to be a physical one.

The disadvantage with the bottom-up troubleshooting approach is it requires that you check every device and interface on the network until the possible cause of the problem is found.

### **Top-Down**
Top-down troubleshooting starts with the end-user applications and moves down through the layers of the OSI model until the cause of the problem has been identified.

End-user applications of an end system are tested before tackling the more specific networking pieces.

The disadvantage with the top-down approach is it requires checking every network application until the possible cause of the problem is found.

### **Divide-and-Conquer**
The network administrator selects a layer and tests in both directions from that layer.

The administrator can work up the OSI layers. If an OSI layer is not functioning properly, the administrator can work down the OSI layer model.

For example, if users cannot access the web server, but they can ping the server, then the problem is above Layer 3. If pinging the server is unsuccessful, then the problem is likely at a lower OSI layer.

### **Follow-the-Path**
The approach first discovers the traffic path all the way from source to destination. The scope of troubleshooting is reduced to just the links and devices that are in the forwarding path. The objective is to eliminate the links and devices that are irrelevant to the troubleshooting task at hand.

### **Substitution**
This approach is also called swap-the-component because you physically swap the problematic device with a known, working one. If the problem is fixed, then the problem is with the removed device. If the problem remains, then the cause may be elsewhere.

### **Comparison**
This approach is also called the spot-the-differences approach and attempts to resolve the problem by changing the nonoperational elements to be consistent with the working ones.

### **Educated Guess**
This approach is also called the shoot-from-the-hip troubleshooting approach. This is a less-structured troubleshooting method that uses an educated guess based on the symptoms of the problem. Success of this method varies based on your troubleshooting experience and ability. 

# Physical Layer Problems

## Common Layer 1 Problems 
Some of the more common Layer 1 problems include the following:

- Device power turned off
- Device power unplugged
- Loose network cable connection
- Incorrect cable type
- Faulty network cable
- Faulty wireless access point

## Wireless Router LEDs 
Regardless of whether the fault is present on the wireless or wired network, one of the first steps in a bottom-up strategy of troubleshooting should be to examine the LEDs, which indicate the current state or activity of a piece of equipment or connection.

Most devices will have activity LEDs, which are often called link lights. A normal condition is for these LEDs to flash indicating that traffic is flowing through the port. A solid green light typically indicates that a device is plugged into the port, but no traffic is flowing. No light typically indicates one or more of the following:

- Nothing is plugged into the port.
- There is an issue with the wired or wireless connection.
- A device or port has failed.
- There is a cabling issue.
- The wireless router is improperly configured, for example, a port was administratively shut down.
- The wireless router has a hardware fault.
- The device does not have power.

## Cabling Problems 
If the wired client is unable to connect to the wireless router, one of the first things to check is the physical connectivity and cabling. 

There are several issues to watch for when cabling:

- Be sure to use the correct type of cable. Two types of UTP cables are commonly encountered in networking: straight-through cables and crossover cables. Using the wrong type of cable may prevent connectivity.
- Improper cable termination is one of the main problems encountered in networks. To avoid this, cables should be terminated according to standards. Terminate cables via the T568A or the T568B termination standard. Avoid untwisting too much of the wire pairs during termination. Crimp connectors on the cable jacket to provide strain relief.
-  Maximum cable run lengths exist based on characteristics of the different cables. Exceeding these run lengths can have a serious negative impact on network performance.
- If connectivity is a problem, verify that the correct ports are being used between the networking devices.
- Protect cables and connectors from physical damage. Support cables to prevent strain on connectors and run cable through areas that will not be in the way.

## Troubleshoot Wireless Issues
Many factors can affect our ability to connect hosts using RF:

- Not all wireless standards are compatible. The 802.11ac (5 GHz band) is not compatible with the 802.11b/g/n standards (2.4 GHz band). Within the 2.4 GHz band, each standard uses different technology. 
- Each wireless conversation must occur on a separate, non-overlapping channel. Some AP devices can be configured to select the least congested or highest throughput channel.
- The strength of an RF signal decreases with distance. If the signal strength is too low, devices will be unable to reliably associate and move data. The signal may be dropped. The NIC client utility can be used to display the signal strength and connection quality.
- RF signals are susceptible to interference from outside sources, including other devices functioning on the same frequency.
- APs share the available bandwidth between devices. As more devices associate with the AP, the bandwidth for each individual device will decrease causing network performance problems. The solution is to reduce the number of wireless clients using each channel.

## Authentication and Association Errors 
Modern WLANs incorporate various technologies to help secure the data on the WLAN. Some of the most common settings that are configured incorrectly include the SSID, authentication, and encryption.

- The SSID is a case-sensitive, alphanumeric string that is up to 32-characters. It must match on both the AP and client. If the SSID is broadcast and detected, this is not an issue. If the SSID is not broadcast, it must be manually entered onto the client. If the client is configured with the wrong SSID, it will not associate with the AP. Additionally, if another AP is present that has broadcasted the SSID, the client may automatically associate to it.
- On most APs, open authentication is configured by default, allowing all devices to connect. If a more secure form of authentication is configured, a key is necessary. If the keys do not match, authentication will fail, and the devices will not associate.
- Encryption is the process of altering the data so that it is not usable by anyone without the proper encryption key. If the client associates with the AP but cannot send or receive data, the encryption key may be the issue.

# Common Internet Connectivity Issues
## Common Internet Connectivity Issues
If the physical connection to the wired or wireless host appears to be connecting as expected but the host cannot communicate on remote networks or the internet, then check the IP configuration of the client.

The IP configuration can have a major impact on the ability for a host to connect to the network. A wireless router acts as a DHCP server for local wired and wireless clients and provides IP configuration, including the IP address, subnet mask, default gateway, and commonly the IP addresses of DNS servers. 

## Check Internet Configuration 
If hosts on the wired and wireless local network can connect to the wireless router and with other hosts on the local network, but not to the internet, the problem may be in the connection between the router and the ISP.

    C:∖> ping 10.18.32.12
    Pinging 10.18.32.12 with 32 bytes of data:
    Request timed out.
    Request timed out.
    Request timed out.
    Request timed out.

    Ping statistics for 10.18.32.12:
        Packets: Sent = 4, Received = 0, Lost = 4 (100% loss),

## Check Firewall Settings 
If Layers 1 through 3 all appear to be operating normally and you can successfully ping the IP address of the remote server, it is time to check the higher layers. For example, if a network firewall is used along the path, it is important to check that the application TCP or UDP port is open and no filter lists are blocking traffic to that port.

If all clients are obtaining the correct IP configuration, and can connect to the wireless router but are unable to ping each other or cannot access a remote server or application, the problem may be with rules on the router. Check all settings on the router to ensure no security restrictions could be causing the issue. Verify that the local firewalls on the client devices are not preventing network functionality.

## Divide and Conquer with ping 
When troubleshooting a network with both wired and wireless connections, it is often best to troubleshoot using a divide-and-conquer technique to isolate the problem to either the wired or the wireless network. The easiest way to determine if the problem is with the wired or the wireless network is to do the following:

- Ping from a wireless client to the default gateway. This verifies if the wireless client is connecting as expected.
- Ping from a wired client to the default gateway. This verifies if the wired client is connecting as expected.
- Ping from the wireless client to a wired client. This verifies if the wireless router is functioning as expected.

## The tracert Command 
The **tracert** utility provides connectivity information about the path a packet takes to reach the destination and about every router (hop) along the way. It also indicates how long a packet takes to get from the source to each hop and back (round trip time). The tracert utility can help identify where a packet may have been lost or delayed due to bottlenecks or slowdowns in the network.

In the figure, the user is tracing the path to Cisco. The path is unique to this user. Your path will have a different listing of hops and may be shorter or longer (number of hops).

> Note: Notice in the output that the 2nd hop failed. This is most likely due to a firewall configuration on that device which does not permit responding packets from the tracert command. However, the device does forward the packets to the next hop.

    C:\Users\****>tracert www.cisco.com

    Tracing route to e2867.dsca.akamaiedge.net [104.64.113.19]
    over a maximum of 30 hops:

    1    <1 ms    <1 ms    <1 ms  192.168.10.1
    2     6 ms     6 ms     6 ms  nsa.nwt.cz [217.197.156.1]
    3     *        *        *     Request timed out.
    4     6 ms     6 ms     6 ms  78.136.132.18
    5   109 ms    46 ms   111 ms  nix4.akamai.com [91.210.16.221]
    6    10 ms     6 ms     7 ms  a104-64-113-19.deploy.static.akamaitechnologies.com [104.64.113.19]

    Trace complete.

> The basic tracert command will only allow up to 30 hops between a source and destination device before it assumes that the destination is unreachable.

## The netstat Command 
Sometimes it is necessary to know which active TCP connections are open and running on a networked host. The netstat command is an important network utility that can be used to verify those connections.

    C:∖> netstat

    Active Connections

    Proto     Local Address          Foreign Address          State
    TCP       10.10.10.130:58520     dfw28s01-in-f14:https    ESTABLISHED
    TCP       10.10.10.130:58522     dfw25s25-in-f14:https    ESTABLISHED
    TCP       10.10.10.130:58523     dfw25s25-in-f14:https    ESTABLISHED
    TCP       10.10.10.130:58525     ec2-3-13-132-189:https   ESTABLISHED
    TCP       10.10.10.130:58579     203.104.160.12:https     ESTABLISHED
    TCP       10.10.10.130:58580     104.16.249.249:https     ESTABLISHED
    TCP       10.10.10.130:58624     52.242.211.89:https      ESTABLISHED
    TCP       10.10.10.130:58628     24-155-92-110:https      ESTABLISHED
    TCP       10.10.10.130:58651     ec2-18-211-133-65:https  ESTABLISHED
    TCP       10.10.10.130:58686     do-33:https              ESTABLISHED
    TCP       10.10.10.130:58720     172.253.119.189:https    ESTABLISHED
    TCP       10.10.10.130:58751     ec2-35-170-0-145:https   ESTABLISHED
    TCP       10.10.10.130:58753     ec2-44-224-80-214:https  ESTABLISHED
    TCP       10.10.10.130:58755     a23-65-237-228:https     ESTABLISHED

    C:∖>

Unexplained TCP connections can pose a major security threat. This is because they can indicate that something or someone is connected to the local host. Additionally, unnecessary TCP connections can consume valuable system resources thus slowing down the performance of the host. 

## The nslookup Command 
When a user application requests to connect to a remote device by name, the requesting DNS client queries the name server to resolve the name to a numeric address.

Computer operating systems also have a utility called **nslookup** that allows the user to manually query the name servers to resolve a given host name. This utility can also be used to troubleshoot name resolution issues and to verify the current status of the name servers.

    C:∖Users> nslookup
    Default Server:  dns-sj.cisco.com
    Address:  171.70.168.183
    > www.cisco.com
    Server:   dns-sj.cisco.com
    Address:  171.70.168.183
    Name:    origin-www.cisco.com
    Addresses:  2001:420:1101:1::a
            173.37.145.84
    Aliases:  www.cisco.com
    > cisco.netacad.net
    Server:  dns-sj.cisco.com
    Address:  171.70.168.183
    Name:    cisco.netacad.net
    Address:  72.163.6.223
    >

# Customer Support
## Support Desk Tickets and Work Orders 
When a Level 1 support desk technician receives a call, there is a process followed to gather information. There are also specific systems for storing and retrieving relevant information. It is extremely important to gather the information correctly in the event that a call has to be escalated to a Level 2 technician, or require an on-site visit.

The information gathering and recording process starts as soon as the technician answers the phone. After customer identification, the technician accesses the relevant customer information. Typically, a database application is used to manage the customer information.

The information is transferred to a trouble ticket, or incident report. This document can be a piece of paper in a paper filing system or an electronic tracking system designed to follow the troubleshooting process from beginning to end. Each person who works on the problem is expected to record what was done on the trouble ticket. When an on-site call is required, the trouble ticket information can be converted to a work order that the on-site technician can take to the customer site.

When a problem is resolved, the solution is documented in the customer work order or trouble ticket, and in a knowledge base document for future reference.
