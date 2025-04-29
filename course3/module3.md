# Cybersecurity Controls

## Learning Objectives
- Define network mapping and discuss its use by both cybersecurity professionals and attackers
- Describe packet sniffing and explain key strategies to protect your network against it
- Describe IP spoofing and various defense mechanisms against it
- Describe denial-of-service (DoS) attacks
- Define injection attacks and outline two prevalent types
- Identify different types of security controls
- Recognize the distinct functions of security controls
- Identify various methods and tools to maintain system security
- Define network security and describe the various tools and methods for securing a network
- Recognize the significance of application security and identify key secure coding practices for enhancing it
- Describe the vulnerability process and identify tools with robust vulnerability assessment capabilities
- Outline the four key phases of the Incident Response (IR) lifecycle and describe the role of digital forensics

## Network Mapping
- Network mapping is the process of understanding and visualizing a network's physical and logical connections.
- Nmap enables administrators to identify the devices operating on their systems, discover open ports, and detect security risks.
- Wireshark is a powerful network protocol analyzer.
- Wireshark provides visibility into the specific network traffic details.

IT and cybersecurity professionals can leverage network mapping to: 
- Manage the network's complexity
- Easily troubleshoot issues
- Detect anomalies in the network
- Proactive network management and strategic planning
- Efficient documentation

The attackers leverage network mapping to:
- Identify unguarded entry points, vulnerable systems, defenses
- Navigate the network
- Prioritize target segments
- Deduce high-value assets
- Craft tailored phishing campaigns, or social engineering attacks

## IP Spoofing
- IP spoofing involves manipulating packet headers to alter the source address, effectively concealing the true origin of the sender or pretending to be another host.
- DDoS commonly employs IP spoofing and floods a target with excess traffic, disrupting services.
- A botnet refers to a collection of interconnected computers centrally controlled by one or more attackers.
- The man-in-the-middle strategy is to intercept the exchange between two systems, modify the packets and then forward them undetected by the authentic communicator or recipient.

## Injection Attacks
- Injection attacks are cyber attacks, where an attacker injects malicious code into a query, web application, or system, triggering remote commands that manipulate website data. 
- There are two popular injection attacks, SQL injection and XSS. 
- Attackers exploit SQL injection vulnerabilities to gain unauthorized access and compromise sensitive information. 
- The major consequences of SQL injection attacks include confidentiality breach, authentication compromise, authorization loss, and integrity violation.
- XSS attacks are security breaches where attackers embed harmful scripts into web pages. 
- There are two types of XSS attacks, server XSS and client XSS.
- IP spoofing poses challenges to law enforcement and cybersecurity teams.
- IP spoofing can be limited using the following techniques;
- Ingress filtering, which establishes a critical network security measure where traffic is inspected and managed at the point of entry to the network
- Egress filtering, which specific networks deploy as an added layer of protection

## Security Controls

- Security controls are essential for safeguarding the confidentiality, integrity, and availability of critical information and other crucial assets from potential threats. 
- There are various security controls that safeguard hardware, software, networks, and data from potential harm.
- These include administrative controls, physical controls, and technical controls.
- When a security measure is implemented, its function is broadly specified into different categories.
- Some of these include deterrent controls, preventive controls, detective controls, and corrective controls.

## System Security

- Computer system is a comprehensive hardware and software setup with all essential components required for performing computing operations.
- System security protects computer systems and their information from unauthorized access, damage, or theft.
- It professionals actively implement a variety of methods and tools to maintain system security, including access controls, encryption, patching, regular backups, system-level firewalls, and antivirus software.

## Application Security by Design

- Software development life cycle is a structured sequence of stages outlining the software development process from the beginning to the end.
- Application security involves incorporating a series of secure practices and processes into every phase of the software creation process. The
- key secure coding practices for enhancing application security include, input validation ,error handling, secure logging, avoid leaving hardcoded credentials, access control, encryption, and software secure testing.

## Vulnerability Management

- The first step in the vulnerability management process is to define and categorize the potential scan targets
- Conduct automated regular scans to detect emerging vulnerabilities as quickly as possible
- It is essential to select tools with robust vulnerability assessment capabilities
- Two notable scanners in the industry are Nessus and OpenVAS
- Application testing uses three techniques; SAST, DAST, and IAST, parameters must be set so that scans probe deep enough to uncover potential vulnerabilities
