# Module 3 - Network Protocols
In this module, you'll learn about network protocols and security measures, combining theoretical knowledge with practical applications. You will begin with an introduction to application and transport protocols, focusing on UDP and TCP. You will then explore DNS and DHCP and experience a hands-on lab for configuring DHCP and an activity on DNS filtering. Then learn how to use Syslog message logs and network analysis techniques, including port mirroring, promiscuous mode, and user behavior analysis.

## Learning Objectives
- Describe how broadcasting domains are used
- Differentiate between collision and broadcast domains
- Describe the event attributes to include in event logs
- Identify the legitimate and illegitimate uses of port mirroring
- Explain how to use flow utilities such as NetFlow to collect and visualize network traffic flow statistics on routing devices
- Define the Syslog protocol
- Describe the dynamic host configuration protocol (DHCP), including the service that it provides
- Describe the domain name system (DNS), including the service that it provides
- Analyze network traffic using techniques such as port mirroring, promiscuous mode, and user behavior analysis
- Differentiate between the TCP and UDP transport layer protocols
- Identify a protocol associated with TCP
- Describe common uses for UDP
- Demonstrate DNS and DHCP installation and configuration
- Explain how user behavior analysis helps secure networks
- Discuss how networks use port mirroring and promiscuous mode
- Discuss how to apply DNS filtering
- Explain network flow, including NetFlow analysis capabilities
- Describe how networks use the Syslog Messaging protocol
- Demonstrate how to configure and manage DNS and DHCP services
- Differentiate between how networks use UDP and TCP transport protocols

## Application and Transport Protocols, Part 1
TCP packet information contains the sender, an identifying recipient, data verification packets, and a list of packets in order. TCP data transmissions include information that enables the receiving computer to verify receipt of all the packets and their order. UDP sends data packets without confirming that the correct computer received the data packets. UDP might send the packet data out of order and not verify that the receiving computer received all the packets. UDP protocols specify source and destination ports to direct data packets to the correct application on a device for proper communications, and FTP, DNS, SNMP, DHCP, VoIP, and IPTV. Use UDP and specific ports for fast efficient data transfer, often prioritizing speed over reliability for file transfers, name queries, IP management, voice communication, and TV streaming.

## Application and Transport Protocols, Part 2
TCP transmission control protocol ensures reliable data transmission by establishing a connection, tracking data packets and requiring acknowledgments. UDP, user datagram protocol offers faster data transmission without establishing a connection or requiring acknowledgments. A three-way handshake includes the sender sending an SYN request, the recipient responding with a SYN-ACK, and the sender replies with an ACK. The components of TCP include source and destination ports, sequence and acknowledgment numbers, and flags, and applications using TCP include HTTP, HTTPS, SMTP, and FTP.

## Exercises
### Exercise 1: Capture and Analyze HTTPS Traffic (TCP)
- Objective: Experience how Hypertext Transfer Protocol Secure( HTTPS) operates over TCP by capturing and analyzing its traffic.
- Open Wireshark using Run as Administrator and start a new capture session.
- In the filter bar, enter tcp port 443 to capture HTTPS traffic
- Open a web browser and visit any secure website (such as https://www.google.com).
- Stop the capture after a few seconds.
- Analyze the captured packets to identify the TCP three-way handshake (SYN, SYN-ACK, ACK).
- Observe the encrypted HTTPS traffic and note the absence of visible content due to encryption, while still understanding the flow of requests and responses.

### Exercise 2: Capture and Analyze DNS Traffic (UDP)
- Objective: Experience how User Datagram Prootcol (UDP) operates by capturing and analyzing its traffic.
- Open Wireshark using Run as Administrator and start a new capture session.
- In the filter bar, enter udp port 53 to capture UDP traffic.
- To generate DNS traffic, type nslookup command in command prompt.
- Stop the capture after a few seconds.
- Analyze the captured data to look for DNS requests and responses. Examine the UDP headers.

### Exercise 3: Capture and Analyze ARP Traffic (Layer 2)
- Objective: Experience how Address Resolution Prootcol (ARP) operates by capturing and analyzing its traffic.
- Open Wireshark using Run as Administrator and start a new capture session
- In the filter bar, enter ARP to capture ARP traffic.
- To enerate ARP traffic, type arp -a command in the command prompt.
- Stop the capture after a few seconds
- Analyze the capture lookng for ARP requests and responses. Examine ARP packet details.
