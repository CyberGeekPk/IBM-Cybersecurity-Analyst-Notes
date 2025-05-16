# Module 1 : Cybersecurity Architecture Overview
In this module, you will be introduced to fundamental principles of cybersecurity including defense in depth, least privilege, separation of duties, security by design, Keep It Simple, Stupid (KISS). You will also be introduced to bad practice Security by Obscurity that can lead to cyberattacks. Next, you will be able to recognize the importance and key concepts related to Confidentiality, Integrity, and Availability, or the CIA Triad. Finally, you will become familiar with roles and how to manage the role security and NIST CSF.

## Five Principles to Follow (and One to Avoid)

### 1. Defense in depth
Defense in depth is trying to create an obstacle course, a difficulty for the bad guy. You can see what I've done here is there's no single security mechanism that is protecting this thing. If any one of these fails, the rest of the system still works. That's the idea that we're after here. If you think about it this way, we've got no single point of failure. We're trying to avoid single points of failure. We want a system that ultimately if it fails, it fails safe. That's what we're trying to get, and that's what the old model and the new model of securities were designed to do. 

### 2. Principle of least privilege
Principle of least privilege basically says, I'm only going to give access rights to people that need that, that are authorized and need it in order to do their job and can justify it, and for only as long as they need that access right.

### 3. Separation of duties
That is, we won't have any single point of control. In fact, what we're trying to do is force collusion by two bad actors or more than two bad actors in order to compromise the system. But no single person can create the compromise. 

### 4. Secure by design
In other words, it shouldn't be an afterthought that we put security in. Security can't just be a bolt on that, you do at the end. In fact, it needs to be something that we're doing throughout pervasively. We look at the security aspects of the requirements, we build security into the design. We are thinking about secure coding principles all the path. When we install, we do it on a secure system, we're testing and guarding that test data. Then the production, obviously we keep testing. Security is something we do throughout. But it doesn't begin here, It begins in these phases. That's what we're really looking for here.
In other words, what we're trying to do is make security start to finish and we want secure by design means it's secure out of the box. That's the way we'd like it to be. Sometimes we're going to have to do some configuration changes to make it more secure, but this is the goal that we're trying to shoot for. Secure by design, secure out of the box.

### 5. KISS principle
It stands for Keep It Simple Stupid. In other words, we don't want to make it harder than necessary, because that will make it easier for the bad guys and harder for the good guys.
The lesson here is if we make it harder to do the right thing than it is to do the wrong thing, people are going to do the wrong thing. So we need to be able to make the system secure but also as simple as possible. Keep it simple stupid. 
What we want to do, is understand complexity is the enemy of security. We want to make the system just complex enough to keep the bad guys out. But not so complex that it's hard for the good guys to do what they need to do.

### Security by obscurity
The security principle you should never observe, and that is security by obscurity. That is, relying on some secret knowledge in order to make the system safe. It turns out that secrecy and security are not the same thing. In fact, what we want is a system that is open and observable and this guy called Kerckhoff came up with what's now known as Kerckhoffs's principle, which basically describes that he was specifically talking about a cryptosystem and he said basically a cryptosystem, should be secure if you know every single thing about it except for the key. In other words, the key is the only secret in the whole system. 
The security doesn't come from some secret knowledge of how this thing works. It's able to produce cipher text from clear text without having to keep this part secret. The only secret is the key, and that's what we want. We do the same things when we talk about secure operating systems or secure applications, or things like that as long as the security is based on secrecy, it's not really something that we can rely on.

# CIA Triad

## Confidentiality
So, confidentiality, we basically accomplish with two main types of technologies: 
One is access control, which consists of authentication and authorization. So authentication is answering the question, "Who are you?" In authorization, "Are you allowed to do this or not?"
Encryption is the other component that is involved in ensuring confidentiality.
So these are two main things then that we're doing. We're using access control and encryption as ways to ensure confidentiality.

### Solutions to Ensure Confidentiality
- Authentication: Passwords, PINs, and multi-factor authentication methods are used to verify the identity of the user
- Authorization: Verify whether the authenticated user should have access to the requested information
- Encryption: Transform readable data into a coded form that prevents unauthorized access to the information

## Integrity
Integrity is the quality that says a message is true to itself. A transaction is true to itself. If it gets modified, then we can detect it. And if it's detected, then we can know not to trust that and we can take the appropriate countermeasures.
How do we keep those from not happening? We're going to use these cryptographic technologies that allow us to see that a record in either of these cases, if someone attempts to modify that, we can see that attempt and we can block it.

### Solutions to Ensure Integrity
- Controls: Help to protect data from unauthorized creation, deletion, or alterations
- Checksum: Verify data integrity by detecting errors that may have been introduced during transmission or storage
- Version control: Record changes to a file over time so that you can see who and when changes were made to the file

## Availability
Availability means that the system should be available, the resources should be available to authorized users--that they can get access when they need it.

### Solutions to Ensure Availability
- Fail-safe mechanisms: Automatically respond to a failure or malfunction to prevent further damage or harm
- Perform regular backups: Routinely create copies of data and store them in a separate location to restore the original data in the event of data loss or disruption
- Disaster recovery plan: Create policies to ensure the rapid restoration of systems, data, and infrastructure in the event of natural disasters, cyber-attacks, and other unforeseen events

![image](https://github.com/user-attachments/assets/5f85d65d-d903-4a9d-b3d3-106e4e9c6271)

# Roles and Tools

## Role and Mindset
AIt all starts with stakeholders providing their requirements to the architect. The architect will develop reference architecture diagrams that show the relations between the high-level components. The architecture diagrams will be translated into an IT architecture diagram.

A simple architecture diagram with a user accessing a device (Desktop/laptop/mobile), which then connects to a web server, which in turn connects with the Application server and accesses a database to retrieve information.
The architect then transfers the information to the engineer, who will implement the system.

Tip: Architect = Whiteboard; Engineer = Keyboard

An architect must understand how a system works to assess how and where the system might fail. Always ask: What do I do to prevent the system from failing? And then figure out how to prevent the failure.

## Commonly Used Tools of the Trade for an Architect
In the case of IT, an architect is creating diagrams. The diagrams act as tools for the architects, and the most common ones are:

- Business Context diagrams provide a high-level line of business view. They show the relationship between different entities in a system.
- System Context diagrams decompose the business context diagram further to determine how the entities might look in a system.
- Architecture Overview diagrams decompose the system context diagrams to determine how the smallest components will look and connect with other components.

The diagrams are part of the architect's vocabulary. They should be designed so that any IT architect could understand them.

A cybersecurity architect will study the diagrams created by the IT architect and determine how to make the systems and overall architecture secure and fail-safe.

The cybersecurity architect will need to use the following as a checklist:

- Five principles of cybersecurity
- CIA triad
- Frameworks, such as NIST CSF, provides a checklist to ensure that you have covered all your bases
As a cybersecurity architect, it is your job to apply all the items in the checklist to the different diagrams and add security components.

It is important to involve the cybersecurity architects in the Risk Analysis phase of a project rather than in the implementation phase. For a secure design and implementation, applying the cybersecurity principles upfront and creating a security policy is important. Then, follow it with an architecture that integrates well with the overall IT architecture.

# NIST CSF
The NIST Cybersecurity Framework (CSF) provides a common language and methodology for organizations to manage and reduce cybersecurity risk. The framework is based on existing best practices, standards, guidelines, and procedures from various government agencies and industry sectors. It consists of the Core, Implementation Tiers, and Profiles. The Core presents common activities and outcomes across critical infrastructure sectors and provides a high-level view of security requirements. The Implementation Tiers help organizations prioritize their efforts by classifying their current cybersecurity risk management approach as Partial, Risk Informed, Repeatable, or Adaptive. Finally, Profiles allows organizations to align cybersecurity practices with business requirements, risk tolerances, and resources.

The CSF comprises five key functions: Identify, Protect, Detect, Respond, and Recover. These functions represent the key components of a successful cybersecurity program and provide a structured approach to managing risk.

![image](https://github.com/user-attachments/assets/7593704f-2da3-42c0-b87b-87d0b1b4e7af)

## 1. Identify
The identify function focuses on understanding the organization's assets, business environment, risk management strategy, and governance structure. This involves identifying all critical assets and data, assessing the potential impact of a cyber-attack on these assets, and determining the organization's risk tolerance level.

This function also includes developing incident response plans, establishing policies and procedures for managing cybersecurity risks, and conducting regular assessments to identify any changes in the organization's risk profile.

## 2. Protect
The protect function involves implementing measures to safeguard the organization's assets and ensure their continued availability, integrity, and confidentiality. This includes physical security controls, access controls, data at rest and in transit protection, employee training programs, and vulnerability management processes.

This function also focuses on supply chain risk management by ensuring that third-party vendors and partners have appropriate security measures to protect the organization's data and assets.

## 3. Detect
The detect function focuses on identifying cybersecurity events and incidents as they occur. This includes implementing monitoring systems, establishing threat intelligence capabilities, and conducting routine assessments of the organization's security posture.

Quickly detecting and responding to cyber-attacks is essential in minimizing their impact on an organization's operations and reputation. Therefore, this function also includes developing incident response plans and conducting regular exercises to test their effectiveness.

## 4. Respond
The respond function focuses on taking appropriate action in response to a cybersecurity event or incident. This may involve containment of the incident, eradicating the threat, and recovering impacted systems or data. It also includes notifying relevant stakeholders, such as customers or regulatory authorities, and implementing additional security measures to prevent similar incidents from occurring in the future.

## 5. Recover
The final function, recover, focuses on restoring operational capabilities and services after a cybersecurity event or incident has occurred. This includes conducting post-incident reviews, implementing changes to policies and procedures, and updating risk management strategies based on lessons learned.

These five functions are not meant to be followed in order. Instead, they should be viewed as a constant process, with each function informing and influencing the others. Implementing the NIST Cybersecurity Framework can help organizations establish a structured approach to managing cybersecurity risk and improve their overall security posture. Because of this, all cybersecurity professionals need to familiarize themselves with the framework.

You can learn more about the NIST cybersecurity Framework here: https://www.nist.gov/cyberframework/getting-started/quick-start-guide.
