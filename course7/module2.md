# Module 2 - Access Management & Endpoint Security
This module introduces Identity and access management (IAM) and endpoints. IAM is one of the security domains and is referred to as the new perimeter. You will learn about the LDAP and the 4 A’s of IAM including administration, authorization, authentication, and audits. After a brief discussion on Privileged access management (PAM), you will be introduced to the concepts of multifactor authentication (MFA) and single sign on (SSO). You will also learn about endpoints, which is another key security domain. After learning the definition of an endpoint, you will be introduced to endpoint management systems, which help control the endpoints.

## Key Takeaways: Identity Access Management

- IAM (Identity and Access Management) is a web service that securely controls access to resources.
### 4As of Identity and access management:
- Administration: It involves determining the current access rights and also creating them. Administration involves creating, updating, and deleting accounts.
- Authentication: It involves determining the identity of the person who needs access.
- Authorization: It involves determining what should be done and what shouldn't be done
- Audit: It involves analysis of the three A's (above) and ensuring that it is adhered to.

- Any information about a user is called identity.
- The place a user identity is saved is referred to as a directory.
- A directory comprises of a database, a schema, a protocol (most commonly used, Lightweight Directory Access Protocol (LDAP)).
### Ways to approach Synchronization:
- Virtual directory: It retrieves the information based on the request sent by the user.
- Meta directory: It takes the information, pre-fetches it, and stores it up to an enterprise directory.
- Privilege Access Management (PAM) monitors and prevents unauthorized privileged access to critical resources.
- A federation capability helps to log in a system as an identity provider and access other systems as a service provider.
- Workforce identity management refers to the processes, tools, and strategies used to manage the workforce.
- Consumer Identity and Access Management (CIAM) is used to integrate both authentication and authorization into customer-facing applications.

## Understanding Multi-factor Authentication
Multi-factor authentication (MFA) is a security mechanism that requires users to provide two or more verification factors to access a resource such as a system, network, or application. This process enhances the security of the protected resource by creating multiple layers of defense against unauthorized access.

## Three factors of multi-factor authentication
MFA is based on the premise that an unauthorized user is unlikely to be able to provide all the required verification factors. These factors are divided into three categories:

- Something you know - This is information known only to the user, such as a password, a PIN, or the answer to a secret question.
- Something you have - This factor involves a physical device in the user's possession. It could be a security token, a bank card, a smartphone, or a hardware dongle.
- Something you are - The most personal factor includes biometric data like fingerprints, retinal patterns, voice recognition, or the user's behavior patterns.

## Single-Factor Authentication (SFA)
is a security process where users provide only one authentication factor to verify their identity, typically a password. If the password is compromised, there's no additional layer of security to prevent unauthorized access. This is the most basic form of authentication, commonly used in personal email or social media accounts.

## Two-Factor Authentication (2FA)
involves two different types of authentication factors. This could be a combination of something the user knows (like a password or PIN), something the user has (like a smart card or mobile device), or something the user is (such as a fingerprint or retinal scan). This method is more secure than SFA as it adds an extra layer of security. Online banking often uses 2FA, requiring a password and a one-time code sent to the user's mobile device.

## Multi-Factor Authentication (MFA)
involves two or more independent categories of credentials to verify the user's identity for a login or other transaction. MFA can include two-factor authentication but also can consist of more. The aim is to create a layered defense and make it more difficult for an unauthorized person to access a target such as a physical location, computing device, network, or database. If one factor is compromised or broken, the attacker still has at least one more barrier to breach before successfully breaking into the target.

## Endpoint Security

- Multi-factor authentication is based on trust in the source platform.
- Endpoints refer to physical devices that connect to a computer network for information exchange.
- Vulnerability can come from both hardware and software devices.
- Visibility and control are keys to security. They dictate the type of hardware and software that are allowed within an organization.
Controls can be in the form of:
-- Inventory
-- Policies
-- Patching
-- Encryption
-- Remote wipe
-- Location tracking
-- Anti-virus
-- Disposal
- Policies are implemented to achieve security. They include passwords (certain length, strength, and expiry date). They also ensure proper encryption.
- Policies should evaluate whether devices are monitored and under what conditions.
