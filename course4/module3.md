# Module 3 : Linux OS

## Learning Objectives
Explain how open-source software, like Linux, fosters transparency, collaboration, and community involvement
Locate system hardware and operating system information and navigate the Ubuntu file system
Explore how the Linux terminal and shell work together to execute commands
Recall common shell commands and shell choices to streamline tasks within the Linux environment
Analyze the Linux directory structure for efficient file management

## Linux Overview
Open-source software has an open license which allows users to view, modify, and distribute its source code freely, Open-source software encourages diversity and customization and offers enhanced security and cost savings.
Linux OS is open-source software that uses a Linux kernel, which serves as the foundation of the OS to manage hardware resources and provide services, Popular Linux distributions include Ubuntu, Fedora, CentOS, Debian, and Linux Mint, And the two main interfaces Linux OS offers are command-line interface (or CLI) and graphical user interface (or GUI).

## Exploring Linux Operating System Essentials
Organizations adopt Linux because of its stability, safety, and efficiency. You first log in as an Administrator to create user accounts. You can set a user account so that the assigned user sets their password the first time they use the workstation. You can select About and click About: View information about your system to view your computer’s name, memory, installed version of Ubuntu, as well as verify operating system updates, and more. To locate files and subfolders, select the Folders icon within the left navigation pane on the Home screen And finally, the System Monitor App organizes system performance information in the Processes, Resources, and File Systems tabs.

## Linux Terminal Overview
A Linux shell is an OS-level application that you can use to enter commands and view the output of those commands. You use a terminal to send commands to the shell. And you can use the cd command to navigate around your Linux filesystem.

## Commonly Used Commands
### File and Directory Operations Commands
- ls - List Files and Directories: With the ls command, users can obtain a detailed listing of files and directories in their current location. This command reveals valuable information such as file permissions, ownership, size, and modification dates.
- pwd - Print Current Working Directory: The pwd command displays the full path of the current working directory, making it easy to ascertain your location within the file system.
- mv - Move and Rename: When you need to reorganize your files or give them a new name, the mv command comes to your rescue. It facilitates both file moving and renaming operations.
- cp - Copy Files and Directories: The cp command is indispensable for duplicating files or creating backups. It allows you to copy files and directories from one location to another.
- rm - Remove Files and Directories: The rm command lets you delete files and directories permanently. Caution is advised, as there is no undo functionality.
- chmod - Change File Permissions: The chmod command is used to control who can read, write, or execute your files. It adjusts file permissions to enhance security.
- chown - Change Ownership: To transfer ownership when another user group needs the file the chown command is employed.

### System Management and Administration Commands
- su or sudo - Switch User and Super User: Elevate your privileges with su (Switch User) or sudo (Super User Do) commands. They empower you to execute commands with heightened permissions, which is crucial for system-wide changes.
- apt-get (sudo) - Package Management (Debian-based): apt-get is your gateway to managing software packages on Debian-based systems like Ubuntu. It assists in installing, upgrading, and removing software with ease.
- yum vs apt - Package Management Dilemma: A choice between yum (RPM-based) and apt (Debian-based) package managers often arises. Each caters to different Linux distributions, such as CentOS and Ubuntu.

### Networking and Connectivity Commands
- ip - Network Interface and Routing: The ip command grants insight into network interfaces and routing, enabling the configuration and troubleshooting of networking settings.
- df - Display Disk Space: The df command provides a comprehensive view of disk usage across various file systems to keep tabs on available disk space.
- grep - Search with Regular Expressions: When searching for specific patterns within files, the grep command, armed with regular expressions, proves invaluable.
- find - Search for Files and Directories: The find command lets you traverse directory hierarchies in search of files and directories matching specific criteria.
- dig - Query DNS Servers: Need to resolve domain names or fetch DNS records? The dig command interfaces with DNS servers, providing valuable information for network management.

### Text Manipulation and Editing Commands
- cat - Concatenate and Display Content: Display the contents of a file using the cat command, essential for quick peeks into file details.
- nano - Text Editing in the Terminal: When a lightweight text editor is needed right from the terminal, nano makes quick edits a breeze.

### Data Archiving and Transfer Commands
- tar - Archive and Compress: The tar command combines files into an archive and optionally compresses them, facilitating efficient storage and transportation.
- rsync - Synchronize Files and Directories: For seamless file synchronization between local and remote systems, the rsync command proves its worth.

### Tab key, paths, and directories
- You do not need to type the full name of the directory. The terminal window can do that for you by typing the first part of its name and then pressing the Tab key. So, the command:
- cd App\<tab\>
- Would result in the command line displaying:
- cd Applications
- Then, press Enter, and you change directories to the Applications folder.

- If you want to access a file in a parent directory, type:
- cd ../\<folder name\>
- The tab key works the same by autocompleting the folder name.
