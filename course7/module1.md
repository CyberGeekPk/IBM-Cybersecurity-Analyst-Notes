# Module 1 : Cybersecurity Architecture Overview
In this module, you will be introduced to fundamental principles of cybersecurity including defense in depth, least privilege, separation of duties, security by design, Keep It Simple, Stupid (KISS). You will also be introduced to bad practice Security by Obscurity that can lead to cyberattacks. Next, you will be able to recognize the importance and key concepts related to Confidentiality, Integrity, and Availability, or the CIA Triad. Finally, you will become familiar with roles and how to manage the role security.

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

![image](https://github.com/user-attachments/assets/5f85d65d-d903-4a9d-b3d3-106e4e9c6271)

### Solutions to Ensure Availability
- Fail-safe mechanisms: Automatically respond to a failure or malfunction to prevent further damage or harm
- Perform regular backups: Routinely create copies of data and store them in a separate location to restore the original data in the event of data loss or disruption
- Disaster recovery plan: Create policies to ensure the rapid restoration of systems, data, and infrastructure in the event of natural disasters, cyber-attacks, and other unforeseen events
