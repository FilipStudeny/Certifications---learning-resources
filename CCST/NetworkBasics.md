# NETWORK BASICS
- Internet - Collection of interconnected networks, cooperating with each other to exchange information using common standards.

### LOCAL NETWORKS
- Network in building
- Network in small offices or home offices => **SOHO** - Small office/home office network

## DATA TRANSMISION
- Data transported as **bits** - 0/1 = "binary digit"

### Common Methods of Data Transmission 
- After data is tranformed into a series of bits, it is send via medium (coax-cable, optical fibre = cables/wirelss)
- 3 Forms of signal transmission
    -   Electrical signals - by copper wires
    -   Optical signals - Fibre cables
    -   Wireless signals - By air 

## BANDWIDTH AND THROUGHPUT
- To support "high bandwidth" applications, network have to be capable of transmitting and receiving bits at very high rate

- Different physical media support transfer of bits at different speeds. The rate of data transfer is usually discussed in terms of bandwith and throughput.

- **BANDWIDTH** 
    - Capacity of a medium to carry data (How much it can carry)
    - Digital bandwidth measures the amount of data that can flow from one place to another in a give amount of time.
    - Mesassured in number of bits that can be sent across media in a second
        - Thousands of bits per second (Kbps)
        - Millions of bits per second (Mbps)
        - Billions of bits per second (Gbps)

    - 1 Byte = 8 bits

| Unit of Bandwidth         | Abbreviation     | Equivalence |
|--------------|-----------|------------|
| Bits per second | bps      | 1 bps        |
| Kilobits per second      | Kbps  | 1 Kbps       |
| Megabits per second      | Mbps  | 1 Mbps      |
| Gigabits per second      | Gbps  | 1 Gbps       |
| Terabits per second      | Tbps  | 1 Tbps       |

- **THROUGHPUT** 
    - Like bandwidth, throughputis the measure of the transfer of vits across the media over a given period of time.
    - Due to a number of factors, throughput does not usually match the specified bandwith.
        - It is affected by:
            - The amount of data being send and received over the connection
            - The type of data being transmitted
            - Latency created by the number of network devices encounetered between source and destination

    - **Latency** refers to the amount of time, including delays, for data to travel from point A to B


    - In an internetwork or network with multiple segments, throughput cannot be faster than the slowest link of the path from sendig device to the receiving device. Even if all or most of the segments have high bandwidth, it will only take on segment in the path with lower bandwith to create a slowdown of the throughput of the entire network.
