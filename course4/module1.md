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
