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

# Transport Layer Overview

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

# Application Layer Overview

## DNS and DHCP
DNS, or domain name system, is a network service that helps translate domain names to IP addresses. DHCP automatically assigns IP addresses to devices, eliminating the need for manual configurations. The DHCP process involves four main messages, discover, offer, request, and acknowledgement. Wireshark captures DHCP packets and helps diagnose issues in the DHCP communication process.

## DNS Filtering
DNS filtering supports cybersecurity efforts by using the DNS system to block access to specific websites or services, including malware. DNS filtering systems check the requested domain against a list of block domains and deny or redirect the request if required. DNS filtering blocks access to malicious sites, preventing cyber threats, infections, and data breaches, and reduces attackers' potential entry points. DNS filtering supports cybersecurity, controls the content, and enhances data privacy. To implement a DNS filtering system, evaluate and select a solution, then deploy, configure, and maintain your system.

## Syslog Message Logging Protocol
The Syslog protocol separates the software that generates messages, the system that stores them, and the software that reports and analyzes those messages. System administrators use Syslog for system management, security auditing, general informational analysis, debugging messages, event notification messages, and forensic research. The Syslog includes a content layer for storing messages, an application layer for message generation, interpretation, routing, and storage, and a transport layer for managing the transportation of Syslog messages across the network. Syslog players include the originator, the collector, the relay server, the transport sender, and the transport receiver. Syslog message components include the facility code, severity level, the originator process ID, timestamp, and the reporting device hostname or IP address.

## Flows and Network Analysis
Network flows provide statistics about packet flow through routers. Network flows collect samples of the flows using devices such as routers and switches, network flow applications report on packet usage, bytes sent, time of day/time stamps, port utilization, QoS, application, routing and pairing, and protocols in use, and the NetFlow dashboard categorizes traffic based on the application that's using the interface, providing bytes of data and packet information.

## Port Mirroring and Promiscuous Mode
Port mirroring helps to analyze data and detect network errors. Remote Switch Port Analyzer, or RSPAN, allows the destination port to be remote. Intrusion detection systems, IDS, help to analyze destination ports and monitor real-time traffic to detect anomalies. Wireshark helps to put NIC in promiscuous mode. 

## User Behavior Analysis
User behavior analysis involves systematic monitoring and detailed analysis of user actions within a network, to identify patterns and anomalies. User behavior analysis concepts include baselining normal behavior, anomaly detection, and contextual awareness. UBA techniques and tools include machine learning algorithms, statistical analysis, and log analysis. Some UBA implementation techniques include data collection, integration with SIEM systems, and continuous monitoring. While implementing UBA, you must remain aware of data privacy concerns, false positives, and scalability. UBA help safeguard companies across industries and user roles from financial to healthcare.

# Summary: Network Protocols

- The key elements of the Transport Control Protocol (TCP) packet include the sender, an identifying recipient, data verification packets, and a list of packets in order. TCP ensures reliable data transmission by establishing connections, tracking data packets, and requiring acknowledgments. The components of TCP include source and destination ports, sequence and acknowledgment numbers, and flags. TCP applications include HTTP, HTTPS, SMTP, and FTP.
- User Datagram Protocol (UDP) sends data packets without confirming that the correct computer received the data packets. UDP protocols specify source and destination ports to direct data packets to the correct application on a device for proper communications. UDP offers faster data transmission without establishing a connection or requiring acknowledgments.
- File Transfer Protocol (FTP), Domain Name System (DNS), Simple Network Management Protocol (SNMP), Dynamic Host Configuration Protocol (DHCP), Voice over Internet Protocol (VoIP), and Internet Protocol Television (IPTV) use UDP and specific ports for fast and efficient data transfer.
- A three-way handshake includes the sender sending a Synchronize (SYN) request, the recipient responding with a Synchronize-Acknowledge (SYN-ACK), and the sender replying with an Acknowledge (ACK).
- DNS is a network service that helps translate domain names to Internet Protocol (IP) addresses.
- DHCP automatically assigns IP addresses to devices, eliminating the need for manual configurations. The DHCP process involves four main messages: Discover, Offer, Request, and Acknowledgment.
- Wireshark captures DHCP packets and helps diagnose issues in the DHCP communication process.
- DNS filtering enhances cybersecurity by using the DNS system to block access to specific websites or services, including malware. DNS filtering systems check the requested domain against a list of blocked domains and deny or redirect the request. To implement a DNS filtering system, evaluate and select a solution, then deploy, configure, and maintain your system.
- The Syslog protocol separates the software that generates messages, the system that stores them, and the software that reports and analyzes those messages. The Syslog includes a content layer for storing messages, an application layer for message generation, interpretation, routing, and storage, and a transport layer for managing the transportation of Syslog messages across the network.
- Syslog players include the Originator, Collector, Relay Server, Transport Sender, and Transport Receiver. Syslog message components include the facility code, severity level, Originator process ID, timestamp, and reporting device hostname or IP address.
- Network flows provide statistics about packet flow through routers. Network flow applications report on packet usage, bytes sent, time of the day/timestamps, port utilization, QoS, application, routing and pairing, protocols in use.
- The NetFlow dashboard categorizes traffic based on the application that's using the interface, providing bytes of data and packet information.
- User Behavior Analysis (UBA) involves systematic monitoring and detailed analysis of user actions within a network to identify patterns and anomalies. UBA techniques and tools include machine learning algorithms, statistical analysis, and log analysis. Some UBA implementation techniques include data collection, integration with Security Information and Event Management (SIEM) systems, and continuous monitoring. 

