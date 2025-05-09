# Module 2 - IP Addressing, Routing & Switching
After completing this module, you will be able to explain and apply IP addressing, IP address structure and network classes, IP protocols, traffic routing, and the IPv6 address schema. You’ll also be able to compare the structure and uses of IPv4 and IPv6. You’ll be able to explain basic network routing principles, Layer 2 and Layer 3 addressing, and Address Resolution Protocols (ARP) and describe the basics of routers and routing table sessions. You'll gain experience you can use in the real world when you learn how to secure a small office/home office (SOHO) network.

## Learning Objectives
- Summarize the structure, characteristics, conversion methods, and limitations of IPv4 addresses across network classes
- Contrast IPv4 and IPv6 addressing
- Describe the purpose of subnet masks and gateways
- Explain how IP addresses work
- Describe IPv4’s four-octet format and the five ranges of IPv4’s classful addressing schema
- Describe the use of routing tables in network routing
- Describe how address resolution protocol (ARP) tables are used
- Distinguish between an IP address and a MAC address
- Distinguish between the Layer 2 and Layer 3 addressing schemes
- Distinguish between static and dynamic IP address translation
- Explain how networks use Layer 2 and Layer 3 network addressing
- Explain the structure and uses for IPv6
- Discuss how networks use binary numbering
- Define IP address structure and network classes
- Describe IP protocols and their relationship with network traffic routing
- Implement network routing and address resolution protocols
- Secure a small office/home office (SOHO) network

## IP Addressing - The Basics of Binary
Decimal operates on base 10, while binary operates on base two. Hexadecimal, base 16 offers a more compact number representation compared to binary. To calculate the number representations by raise the base to the power of the number of digits available. To convert from any base system to decimal, draw a table where column headers represent the base raised to increasing powers.

## IP Address Structure and Network Classes
IPv4 or Internet protocol version 4 is the foundational protocol used for identifying and locating devices on networks since its introduction in 1983. It utilizes a 32-bit addressing scheme divided into four octets, each representing a segment of the address, crucial for network and host identification. Class A, B, C, D, and E networks categorize addresses based on their range and intended use from unicast communication to multicasting and experimental purposes. Despite its widespread adoption, IPv4 faces challenges such as address exhaustion due to the rapid growth of Internet connected devices, prompting the development of IPv6.

## IP Protocol and Traffic Routing
Internet protocol, IP, and IP addresses, route data packets within networks and across the Internet for reliable communication. Routable protocols like IP can be routed outside the originating network. Understanding subnet masks and default gateways is crucial. The IP protocol header includes the version, IPv4 or IPv6, and other elements necessary for packet inspection and processing. Source IP addresses identify the sender and destination IP addresses indicate where the packet is being sent. Network masks divide an IP address into network and host segments. The prefix indicates the number of bits used for the network portion. Default gateways forward packets outside the local network, managing traffic between internal and external systems. Broadcast IP addresses have all host portion bits turned on, allowing communication to all devices in a network segment.

## Introduction to the IPv6 Address Schema
IPv6 extends IP addresses from 32 bits to 128 bits, vastly increasing the number of possible addresses. IPv6 addresses use eight groups of four hexadecimal digits separated by colons. In IPv6, a double colon can replace consecutive zeros in an address, but can only be used once. IPv6 headers are simpler and more efficient than IPv4 headers, improving processing speed. IPv6 supports unicast, multicast, and Anycast, replacing IPv4's broadcast method with Anycast.

## Exercises
### IPv4 Exercises
#### Exercise 1: IPv4 Subnet Mask Calculation

Instructions
Given an IP address and a CIDR prefix, determine the subnet mask in decimal format.

Given

IP Address: 172.16.0.0/20
Hint:
The /20 notation means the first 20 bits are for the network portion. Convert this to a decimal subnet mask.

#### Exercise 2: IPv4 Subnet Calculation

Instructions
You need to divide a given network into smaller subnets. Calculate the new subnet mask and list a few resulting subnets with their address ranges.

Given

Network Address: 192.168.10.0/24
Required Subnets: 8
Hint
To create 8 subnets, you'll need to borrow a certain number of bits from the host portion. Adjust the CIDR notation accordingly and determine the new subnet mask.

### IPv6 Exercise
#### Exercise 1: IPv6 Subnetting

Instructions
You are given an IPv6 address and need to create subnets. Calculate the new subnet mask and list a few of the resulting subnets.

Given

IPv6 Address: 2001:abcd:1234::/48
Required Subnets: 4
Hint
To create 4 subnets, you need to borrow 2 bits from the host portion. Adjust the CIDR notation and subnet mask accordingly.

## Basics of Network Routing
Layer 2 addresses or MAC addresses are embedded in network interface cards and serve as physical identifiers. Layer 3 addresses or IP addresses are used for logical addressing across networks. The ARP process ensures that data sent to an IP address reaches the correct device within a local network, and routing tables help determine the best path for data packets.

## Layer 2 and Layer 3 Addressing
Network interfaces may be a single chip or a whole network interface card, commonly referred to as NIC. MAC spoofing is used to bypass MAC address filtering by setting up on a firewall to protect assets. MAC address is 48 bits long or a string of 48, ones and zeros, divided into six octets or six groups of eight bits each. Broadcast domains can also be called virtual LANs or VLANs.

## Address Resolution Protocol
Address resolution protocol, ARP is pivotal in networking, translating IP addresses to MAC addresses for effective data transmission across devices within the same broadcast domain. The ARP table, accessible through commands like ARPA, provides crucial mappings of IP addresses to MAC addresses, aiding and troubleshooting the network management across different operating systems. MAC addresses are essential for transmitting data within the same broadcast domain or local network.
Networks are interconnected through routers spanning multiple broadcast domains. Packet delivery across networks is facilitated by configuring default routes and maintaining ARP tables. Routing tables within routers are crucial for determining the most efficient paths for packet forwarding. ARP tables play a key role in routers by mapping IP addresses to MAC addresses for devices on the same network. Routers enhance communication between departments by facilitating reliable document transfer across distinct network segments. [MUSIC]
Default routes serve to forward packets to destinations, not explicitly listed in the routing table, ensuring connectivity, even when specific network details are unknown. Directly connected routes indicate networks accessible through a router's interfaces, simplifying communication within immediate network segments. Dynamic routes managed through protocols like OSPF and EIGRP, automate route updates based on network conditions, enhancing efficiency and adaptability in complex network environments. Networks determine packet forwarding paths using routing tables, directing traffic based on destination IP addresses.

## Summary: IP Addressing, Routing and Switching
- An IP address is a dotted-decimal number involving binary numbers with a base 2. These binary numbers can be converted to octal, decimal, and hexadecimal number systems with bases 8, 10, and 16.
- To calculate the number representations, raise the base to the power of the number of digits available.
- To convert from the base system to decimal, draw a table in which column headers represent the base raised to increasing powers.
- Since its introduction in 1983, Internet Protocol Version 4 (IPv4) has been the foundational protocol for identifying and locating devices on networks.
- It utilizes a 32-bit addressing scheme divided into four octets, each representing a segment of the address, crucial for network and host identification.
- Class A, B, C, D, and E networks categorize addresses based on their range and intended use, from unicast communication to multicasting and experimental purposes.
- Despite its widespread adoption, IPv4 faces challenges such as address exhaustion due to the rapid growth of internet-connected devices, prompting the development of IPv6.
- Internet Protocol (IP) and IP addresses route data packets within networks and across the internet for reliable communication.
- Routable protocols, like IP, can be routed outside the originating network; understanding subnet masks and default gateways is crucial.
- The IP protocol header includes the version (IPv4 or IPv6) and other elements necessary for packet inspection and processing.
- Source IP addresses identify the sender, and destination IP addresses indicate where the packet is sent.
- Network masks divide an IP address into network and host segments; the prefix indicates the number of bits used for the network portion.
- Default gateways forward packets outside the local network, managing traffic between internal and external systems.
- Broadcast IP addresses have all host portion bits turned on, allowing communication to all devices in a network segment.
- IPv6 extends IP addresses from 32 bits to 128 bits, vastly increasing the number of possible addresses.
- IPv6 addresses use eight sets of four hexadecimal digits, each set separated by colons.
- In IPv6, a double colon can replace consecutive zeros in an address. IPv6 headers are simpler and more efficient than IPv4 headers, improving processing speed. IPv6 supports Unicast, Multicast, and Anycast, replacing IPv4's broadcast method with Anycast.
- Network interfaces may be a single chip or a whole network interface card, commonly called NIC.
- Mac spoofing bypasses MAC address filtering by setting up a firewall to protect assets.
- A MAC address is 48 bits long, or a string of 48 1s and 0s divided into 6 octets or 6 groups of 8 bits each.
- Broadcast domains can also be called virtual LANs (VLANs).
- Address Resolution Protocol (ARP) is pivotal in networking. It translates IP addresses to MAC addresses for effective data transmission across devices within the same broadcast domain.
- The ARP table, accessible through commands like arp -a, provides crucial mappings of IP addresses to MAC addresses, aiding in troubleshooting and network management across different operating systems.
- MAC addresses are essential for transmitting data within the same broadcast domain or local network.
- Routing tables are crucial in directing and optimizing network traffic within organizations, ensuring seamless communication across different departments and buildings.
- Specific network interfaces (enp0s9, enp0s8, enp0s3) handle traffic within their respective broadcast domains, while switches use MAC tables for efficient packet delivery based on MAC addresses.
- Networks are interconnected through routers spanning multiple broadcast domains.
- Packet delivery across networks is facilitated by configuring default routes and maintaining ARP tables.
- Routing tables within routers are crucial for determining the most efficient paths for packet forwarding.
- ARP tables play a crucial role in routers by mapping IP addresses to MAC addresses for devices on the same network.
- Routers enhance department communication by facilitating reliable document transfer across distinct network segments.
- Default routes serve to forward packets to destinations not explicitly listed in the routing table, ensuring connectivity even when specific network details are unknown.
- Directly connected routes indicate networks accessible through a router's interfaces, simplifying communication within immediate network segments.
- Dynamic routes, managed through protocols like OSPF and EIGRP, automate route updates based on network conditions, enhancing efficiency and adaptability in complex network environments.
- Networks determine packet forwarding paths using routing tables, directing traffic based on destination IP addresses.

