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

# Application Security

Every software is prone to vulnerabilities, which are mostly developed in coding stages. This is because traditional software processes are linear and lacks communication. DevOps was introduced because of these reasons.
Short for development, security, and operations, DevSecOps helps to automate every phase of the SDLC. It is an integrated process built for agility.
Secured coding processes involves:
- Coding practices checklist that helps to understand how a code should be written. It also deals with buffer overflow and establishes authentication practices.
- Visit OWASP.ORG for a checklist sample.
- Trusted libraries to eradicate the need of writing a code from scratch.
- Standard architectures references to avoid repeating the same mistakes and learn from them.
- Avoiding vulnerabilities.
- Visit OWASP.ORG and check their list of top ten vulnerabilities.

The idea of a software bill of materials and their details that include:
- Components
- Libraries and their sources
- Dependencies among the components
- Versions
- Vulnerabilities (refer Log4J)
- Static Application Security Testing (SAST) and Dynamic Application Security Testing (DAST) are the two tools used in vulnerability testing. Static is also referred to as white box testing and dynamic testing is referred to as black box testing.

# Secure Coding Practices

## Introduction
Secure coding refers to the practice of developing computer software in a way that guards against security vulnerabilities. Code vulnerabilities are a leading cause of software security breaches. With the increasing reliance on software systems in industries such as finance, healthcare, and defense, the potential damage caused by a security breach can be catastrophic. Secure coding practices can significantly reduce these risks. Secure coding also helps organizations comply with regulatory standards and avoid costly fines or reputational damage associated with security breaches.

Let's look at a few secure coding best practices.

## Input Validation
Input validation determines the correctness of the data that a user or application submits to an application or system. It involves checking whether the user-provided data is of the expected format and free of malicious code. A simple example of input validation is CAPTCHA. This is used to verify that a real person has entered their username and password, reducing the chance of granting access to an AI or a bot. Format checking or regular expressions are another method that checks data against a particular format. For example, an email field may be expecting a 'username@domain' format, or a phone number may be expecting a 'xxx-xxx-xxxx' format.

Inadequate input validation is a common cause of security vulnerabilities, including SQL injection and cross-site scripting attacks. Input validation can help to prevent unauthorized data, maintain the integrity of the system, and mitigate the risk of a potential security breach.

## Authentication and Authorization
Authentication and authorization are two crucial components in secure coding practices. Authentication verifies the identity of a user, device, or system. It ensures that users are who they claim to be before accessing a specific system or data. This often involves using passwords, two-factor authentication, biometric data, or other forms of identity verification.

A robust authentication mechanism can significantly reduce the risk of unauthorized access, thereby maintaining the system's integrity and safeguarding sensitive information.

Authorization pertains to the permissions or privileges granted to a user, device, or system after they have been authenticated. It determines what a user can do or what resources or tasks they can access within the system or application.

Implementing a strict authorization mechanism helps to ensure that users can only access data and perform actions relevant to their role or purpose. This helps to minimize the potential for malicious insider activities or accidental misuse of sensitive data.

## Encryption
Encryption is pivotal to the ethos of secure coding practices. It refers to converting plaintext information into an unreadable form, known as ciphertext, to prevent unauthorized access. The original data can only be reaccessed through decryption, which requires a specific key. Secure software systems often use encryption when storing sensitive data and during data transmission across networks. This ensures that even if an unauthorized party intercepts the data, they cannot comprehend or use it without the decryption key. Encryption is essential in protecting the confidentiality and integrity of data, making it a vital part of secure coding practices. From securing user passwords to safeguarding financial transactions, the significance of encryption in maintaining a robust, secure software environment cannot be overstated.

## Error Handling
Error handling involves anticipating, detecting, and resolving programming errors or exceptions. It ensures that a software application continues functioning as expected, even when an unforeseen issue arises.

In secure coding, error handling becomes especially relevant when dealing with unpredicted or incorrect user inputs or system failures. According to OWASP, developers should ensure that error messages do not display any debugging or stack trace information. Error logs should contain all critical log event data but should not include sensitive data. These logs should only be accessible to unauthorized users. If a user or system can see error logs, they may be able to gain the information needed to infiltrate your system.

Implementing effective error handling can help prevent an application from crashing or exposing sensitive system information when an error occurs.

## Threat Modeling
Threat modeling is a systematic process used in secure coding that involves identifying, understanding, and addressing potential security threats in a software system. It is generally performed at the early stages of development and throughout the software life cycle:

- The process starts by creating a detailed overview of the system — mapping out the data flow, identifying potential vulnerabilities, and defining key areas that threats could target.
- The next step is identifying and categorizing potential threats using STRIDE (Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, and Elevation of Privilege).
- Each threat is then analyzed to understand its potential impact and likelihood of occurrence.
- Appropriate mitigation strategies are then designed and implemented to address each identified threat.
- Regular reviews and updates are carried out as the system evolves and new threats emerge.
- Threat modeling allows for proactive identification and mitigation of potential security risks. It helps prioritize security measures based on the severity and likelihood of threats, significantly reducing the risk of security breaches.

## Secure Code Review
Secure code review is a systematic examination of an application's source code to spot potential security weaknesses and improve the overall quality of the code. A secure code review involves inspecting the code line-by-line to identify any code fragments that may pose a risk of vulnerabilities. It can be conducted manually or automated using tools that detect potentially insecure code patterns.

A secure code review allows developers to catch and correct security flaws early in development.

# Data Security
Data security ecosystem comprises the following:

Governance plan to analyze what should be done. It needs a data security policy to identify the key and sensitive areas:
- Classification criteria to identify key issues and label them (confidential, unclassified, top secret, and so on)
- Catalog to locate the data, especially the sensitive information
- Resilience plan to plan for recovery in case of data breach

Discovery to find sensitive data

- Databases that contain structured data
- Files, emails, and spreadsheets that contain unstructured data

Protection of data

- Encryption that requires data scrambling (for data in databases or in the network)
- Managing the keys and creating them at random
- Access control, which is a part of identity and access management
- Backup to cope with a disaster recovery scenario

Complying with industry regulations

- Looking for general protection guiding bodies (GDPR Europe and HIPAA US)
- Reporting when non-complying with these bodies
- Retaining records in accordance with the law

Security comprises detection

- Monitor the systems and analyze how data is used and by whom
- UBA (User Behavior Analytics) to monitor users and how they perceive data
- Alerts that go to consoles and seek immediate action

Response to security breach

- Investigating cases
- Dynamic playbook for situation handling
- Automation and Orchestration of the cases
= Data Loss Protection (DLP) is a technology that helps to discover the data issues that are flowing across networks.

Five areas that can remove the cost of data breach:
- Artificial intelligence
- DevSecOps
- Incident Response (IR)
- Cryptography
- Employee training

# Data Security: Why a Proactive Stance is Best

## Data preservation
Data preservation, which involves safeguarding critical information from corruption, harm, or loss, is paramount due to the severe consequences of data breaches. These breaches, often resulting from cyberattacks, may include personally identifiable information (PII), health records, financial data, intellectual property, and other personal data. The implications for organizations can be catastrophic, and individuals may suffer significant consequences such as financial losses, identity theft, other forms of fraud, emotional distress, and potential damage to their reputation. Integral to a proactive approach to data security is data privacy, which focuses on how data is stored, accessed, and protected from inappropriate access, theft, or other forms of loss. A compelling example of the significance of data privacy can be seen in the healthcare industry, where maintaining patient confidentiality is essential for building trust and ensuring regulatory compliance.

## Data security strategy
Data security is crucial to safeguarding digital information from threats such as unauthorized access, corruption, theft, accidental disclosure, alteration, and loss. It involves many processes and tools designed to protect an organization's data across various platforms and applications, both within the premises and in the cloud. The goal is to uphold the data's confidentiality, integrity, and availability (CIA) throughout its lifecycle. This includes securing proprietary information, trade secrets, and other sensitive data. A robust data security strategy encompasses the physical security of servers and user devices and the management and control of access, application security, patching, and maintaining reliable data backups. Additionally, it involves employee education and the deployment of a comprehensive suite of threat management, detection, and response tools that protect sensitive data across hybrid cloud environments.

## Data security compliance
In the wake of escalating public anxiety regarding data privacy, governments across the globe are enacting rigorous compliance regulations. The risks of data breaches or losses, audit failures, or regulatory compliance infringements can tarnish an organization's reputation, endanger intellectual property, and result in hefty fines. For example, data breaches under the EU's General Data Protection Regulation (GDPR) could cost an organization up to 4% of its annual global turnover or 20 million euros—whichever is higher. Penalties for non-compliance with data privacy laws can also be severe in the US, with HIPAA Privacy Standards violations attracting fines from $1000 to $50,000 per violation. The Federal Trade Commission (FTC) could impose penalties up to $40,000 per violation of the FTC Act or the Children's Online Privacy Protection Act (COPPA), with each day of non-compliance constituting a separate violation and fine.

## A proactive stance
Firms must adopt a forward-thinking stance on data security, as the financial losses from a breach can be devastating. In 2022, the average time to detect and rectify a data breach was 277 days. Reducing this period to 200 days or fewer could save roughly $1.12 million. Due to stolen or compromised credentials, the most prevalent type of breach costs businesses an additional $150,000 compared to other data breaches. It requires the longest time to detect, averaging 327 days. Implementing a transparent, thoughtful strategy for accessing, curating, classifying, and distributing data throughout the organization bolsters compliance and fosters more informed, data-centric decision-making processes. The greater an organization's knowledge and protection of sensitive data, the more effectively it can leverage it for novel projects and enhance its innovative capacity.
