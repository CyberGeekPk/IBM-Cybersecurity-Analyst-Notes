# Module 3 - Network, Application and Data Security
In this module, you will be introduced to security in the network, application and data domains. As part of the network security domain, you will gain insight into firewall concepts, such as packet filter, stateful packet inspection, and proxy. You will also be introduced to security concepts associated with segments and VPNs, and SASE. Moving to the Application security domain, you will get familiar with the phases when security vulnerabilities creep in along with best practices for secure coding along with introduction of vulnerability testing. The concept of DevSecOps, Static Application Security Testing (SAST) and Dynamic Application Security Testing (DAST) will also be introduced. This module will conclude with concepts associated with data security including governance, discovery, compliance, detection, and response.

## Network Security
Network security helps to protect the usability and integrity of data using firewalls to differentiate between trusted and untrusted networks.

- Packet filtering helps to pass or block data packets in a network using firewalls.
- Data packets contain information on the source address, the destination address, and the port to use.
- Stateful packet inspection helps to evaluate the packets that can be allowed through the firewall. It also looks at the packet contents.
- An application firewall helps to monitor and control the incoming and outgoing network traffic that follows a set of predefined rules.
- A proxy acts on behalf of another party or format. It helps to inspect and enforce a security policy on data.
- Network Address Translation (NAT) helps to map multiple IPs to one another. It helps improve security by translating an internal address that cannot be routed across the internet.
- Virtual Private Networking (VPN) provides a secure channel over an untrusted network. A secure shell is an example of a VPN.
- IPSec is implemented in the network layer to encrypt the communication between two network addresses.
- Secure Access Service Edge (SASE) combines VPN and other networks and delivers them as a single cloud service.
- Data Loss Prevention (DLP) is the practice of detecting and protecting data breaches.

## Securing Network Infrastructure

### Local Area Newtwork
A Local Area Network (LAN), in a network diagram, is usually depicted as a cluster of devices, such as computers, printers, and servers, which are interconnected. The LAN is typically located at the core of the network diagram.

### Modem
The modem typically sits at the network's edge since it is the gateway between the local network and the internet. It is usually connected directly to the internet service provider's line (like a cable or DSL line). From the modem, a line is drawn to a router, which then connects to other devices in the network, like computers, printers, and switches. This setup allows all devices on the local network to access the internet through the modem.

### Router
Routers typically occupy a central role, connecting distinct networks. They are often depicted as nodes between the network's internal segments (such as LANs) and external networks (like the Internet).

Where multiple routers are involved in more complex networks, they are usually shown in the diagram, forming a path between the network's edge (where it interfaces with external networks) and its core (where the most critical, high-capacity parts of the network are located). These routers facilitate data flow, directing traffic based on the most efficient route to ensure seamless network communication.

### Switch
A Switch is usually placed at the heart of the network infrastructure. It is a controller connecting devices like computers, printers, and servers within a local area network (LAN). The switch manages traffic flow in this central role, effectively facilitating communication among connected devices. It often connects to a router, which links the internal network to external networks such as the Internet. The positioning of the switch ensures efficient data transfer within the network, promoting optimal performance and response time.

### Firewall
A Firewall is strategically positioned at the front line of a network, acting as a security control point between the internal network (protected) and external network (unprotected, such as the Internet). The firewall is typically placed immediately after the router to filter incoming and outgoing traffic based on predefined security rules. The placement of the firewall is critical as it ensures that all traffic entering or leaving the network passes through it, adding a crucial layer of security. Its job is to scrutinize all data packets, permitting or denying traffic based on the network's security policies, effectively protecting the network from potential threats.

### Demilitarized Zone (DMZ)
A DMZ in a network diagram is typically placed between the internal protected network (LAN) and an external network, most frequently the Internet. It acts as an additional protective layer, hosting services that communicate with external networks, thus isolating them from the internal, more secure network. Its graphical representation sits between the internal network router and the external-facing router, creating a buffer zone. This architecture reduces the risk of an outside security threat reaching the core components of the internal network.

The DMZ typically hosts systems that provide services to users in external networks such as the Internet. These include Web Servers, which deliver web pages to users who request them via browsers. An Email Server might also be in the DMZ to manage incoming and outgoing mail. Furthermore, a DNS Server, which translates domain names into IP addresses, can be found in the DMZ to aid in resolving external requests. Additionally, FTP Servers for file transfers and VPN Servers for remote network access are often placed in the DMZ. By isolating these servers in the DMZ, organizations seek to limit potential damage from external threats, as these are the systems that primarily interact with the internet and are thus more exposed.

### Intrusion Detection System (IDS)
An IDS in a network diagram is often situated at critical points where it can monitor and analyze traffic to and from all devices on the network. Typically, the IDS is positioned behind the firewall before the network switch to examine internal traffic for any anomalies or patterns that indicate a possible intrusion. Multiple IDS may be used and placed at various entry and exit points in more extensive networks to maximize coverage and protection. The IDS enhances a network's security by providing an additional layer of detection beyond the firewall and DMZ, potentially identifying and alerting to threats these other security measures missed.

### Wireless Router
A Wireless Router is typically situated at a strategic point in a network diagram. This device serves as a router and a wireless access point. It connects wired networks to wireless devices and the internal network to external networks like the internet. The wireless router effectively extends network access to devices that may not be physically wired into the network, enabling them to communicate and share data with other devices on the network. Its position in the diagram reflects its critical role in managing and facilitating wired and wireless communications within the network.
