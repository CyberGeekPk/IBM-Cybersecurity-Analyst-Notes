# Module 2 - Windows Security

## Active Directory Accounts and Security Considerations
- AD functions as a comprehensive organizational tool within Windows Server environments.
- A Domain Admin account holds significant authority and control within an AD domain.
- In a Windows server environment, user accounts play a crucial role as unique identifiers for system access.
- Windows server operating system or OS, supports various types of user accounts.
- Default local accounts serve certain key functions.

## Windows Security Settings
UAC features enhance security and protect against unauthorized changes and malware, BitLocker encrypts system and data drives, while BitLocker to Go extends BitLocker encryption to removable storage devices, and EFS automatically encrypts and decrypts files and folders on NTFS volumes.

## User Management and Permissions
User accounts and groups provide a way to control authentication and access to files, folders, applications, and network services. The difference between running an application or command as an administrator versus a standard user on Windows lies in the level of permissions and privileges granted to each account type. You should use NTFS to set permissions on individual files and folders within an NTFS partition, and use share permissions to provide access to shared folders over a network.

## Antimalware Tools and Microsoft Windows Firewall Configuration
- Microsoft Defender Antivirus is a built-in antivirus solution provided by Microsoft for Windows 10 and Windows 11 operating systems.
- It is crucial to keep your antivirus and anti-malware software up-to-date.
- Software firewalls protect your computer by tracking and controlling network communication.
- The Windows firewall help safeguard your computer by controlling network access and filtering incoming and outgoing traffic.
- Social engineering attacks aimed to deceive individuals into revealing sensitive information, providing unauthorized access, or performing actions that compromise security and user education in the form of anti-phishing training should be an ongoing process.

## Overview of Patching
- Patches address bugs and vulnerabilities post-release, while updates introduce new features.
- Patches and updates protect against cyberattacks and ensure the software works well with new technology.
- Critical software should have security patches applied as soon as released.
- Patch management includes identifying, acquiring, installing, and verifying software applications and system patches.

## Kerberos
- Kerberos is an authentication protocol used across insecure networks like the internet to securely exchange service requests between trusted entities.
- KDC performs two essential operations: user authentication and ticket issuance.
- Kerberos leverages a system of three secret keys: client or user hash, TGS secret key, and service server secret key.
- The protocol involves authentication request initiation, credential verification, message decryption for session keys, and mutual authentication for secure communication.

  
