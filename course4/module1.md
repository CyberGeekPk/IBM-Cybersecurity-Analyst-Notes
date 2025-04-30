# Module 1 - Windows OS
In this module, I learned about file systems and the directory structure of the Windows operating system, how Windows separates 32-bit and 64-bit applications. The module also enable me to explore Windows user mode and kernel mode components. Finally, I have the opportunity to manage Windows files and folders, explore Microsoft Windows server features, and use Microsoft Windows command prompt tools for administration through hands-on labs.

## Learning Objectives
- Use Microsoft Windows command prompt tools for system administration tasks
- Define Active Directory and explain its importance in managing computer systems and network resources
- Use the Microsoft Windows directory structure and file system for effective data management
- Differentiate between 32-bit and 64-bit Windows operating system architectures to select the appropriate system for your computing needs
- Compare and contrast Windows user mode and kernel mode components to troubleshoot issues effectively

## Microsoft Windows Systems Overview
- Windows 10 is an adaptable OS used across various devices and it receives ongoing updates for new features, security, and performance improvements.
- Home users and retailers use Windows 10 Home as their personalized OS.
- Small and medium-sized businesses use Windows 10 Pro for its enhanced data security and centralized control features.
- Large organizations use Windows 10 Enterprise for the tools that deliver security, network optimization, and user customization.
- High-end desktop and workstation professionals use Windows 10 Pro for its high-performing computing capabilities.
- Windows 11 Home provides enhanced security features that are not available in Windows 10 Home.
- Windows 11 Pro offers the same security as Windows 11 Home plus additional security enhancements.
- Large and medium-sized organizations use Windows 11 Enterprise for its advanced security and comprehensive management skills.
- Windows 11 Pro for Workstations is built to handle projects that involve intense graphics work and massive data crunching.

## File Systems
- File systems serve as the foundation for accessing and organizing files across various devices.
- Metadata containing file details like size and permissions helps in maintaining data integrity within file systems.
- The hierarchical structure of file systems allows for easy navigation and organization.
- The FAT system, initially designed for simplicity, operates seamlessly across different platforms.
- NTFS is the standard operating system for Windows and supports advanced features such as file permissions and encryption for enhanced security.

## Directory Structure
- Windows organizes its files hierarchically, like a tree with the C drive as the root. 
- Key directories include users for storing personal data and windows for system files.
- Subdirectories, like System32 and WoW64 contain the system and application files necessary for 32-bit and 64-bit operations.
- Windows maintains hidden files and folders to prevent accidental modification or deletion by users.
- Examples include PerfLogs, pagefile.sys and hiberfil.sys.
- 32-bit systems are limited to 4 gigabytes of memory, which can cause performance issues when running new software.
- 64-bit applications can use way more memory enabling faster processing of large data sets.

## User and Kernel Modes
- The processor in the Windows based computer operates in two different modes, user mode and kernel mode.
- User mode runs applications in a secured environment, preventing direct access to hardware and system components.
- Kernel mode allows the operating system and its components to directly interact with hardware.
- In user mode, each code gets a unique virtual address space, whereas in kernel mode, codes share a single virtual address space.
- Communication between user mode and kernel mode is essential for the smooth functioning of the Windows system.
- The operating system running in kernel mode acts on behalf of the application to perform hardware related tasks through a system of calls known as system calls.

## Microsoft Windows Server Overview
- Microsoft Windows Server, an operating system designed specifically for servers, is a comprehensive and reliable OS for building and managing server infrastructure.
- Network services are designed to streamline network management and enhance security.
- The key features of network services include DNS, DHCP, VPN, and RDS.
- Security and access control in the Windows Server OS help to safeguard resources, data, and user identities.
- The key components of security and access control include Windows firewall, active Directory, RMS BitLocker, and RBAC.


## Microsoft Windows Command Prompt Tools for Administration
- Command prompt, also called the Command-Line Interface, or CLI, is a text-based interface for Microsoft Windows OSs that lets you interact with the system by executing commands.
- The two most common OS user accounts are standard and administrator.
- Standard accounts are the Windows default and are used for regular everyday tasks. And administrator accounts provide elevated privileges like installing software, changing system settings, and running CLI tools.
- Running Command Prompt Tools lets the system carry out actions that require elevated permissions.
- Group Policy lets system administrators manage and control user and computer settings on a network.
- Drive letters identify storage devices on the computer.
- The system maintenance and information commands allow you to manage and maintain a Microsoft Windows OS. Managing files and directories helps you organize and maintain your computer's file system.
- File copying and backup tools allow you to copy files or perform advanced file-copying tasks.
- And hostname and network commands provide information and tools to help you manage and troubleshoot network connections and identify devices on a network.

## Microsoft Management Console
- The Microsoft Management Console (or MMC) is a user interface provided by Microsoft that allows you as an administrator to customize your environment with MMC tools or snap-ins
- MMC enables administrators to use multiple snap-ins on one interface
- MMC provides a customizable environment where you can organize your snap-in tools based on your workflow
- MMC supports role-based administration, which allows you to assign snap-in tools to specific users and groups
- Microsoft Windows provides ten built-in snap-in tools, which simplify system management with the following tools:
- Computer management, group policy management, services, task scheduler, performance monitor, event viewer, device manager, certificate manager, local users and groups, and disk management.

## What is Active Directory
- Active directory helps administrators manage user accounts, computer systems, and network resources in a centralized way on a network
- Administrative features in active directory include Organizational Units, called OUs, Home Folders, Folder Redirection, and Security Groups
- The structure of active directory uses domains, trees, and forests
