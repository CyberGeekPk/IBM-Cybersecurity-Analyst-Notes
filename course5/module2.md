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
