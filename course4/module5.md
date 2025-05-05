# Project overview - System Administration and Security

## Scenario:
Cyber Secure Inc. recently hired you as a junior cybersecurity analyst. Other businesses contract Cyber Secure Inc. to handle their system administration and security.

Suppose my supervisor assigned me six tickets; the first three require work with Windows OS, and the other three require me to work with Linux.

The project has two parts. For part 1, I will use the Rhyme lab environment in Coursera, which emulates a Windows Operating System. 
For part 2, I will use the Skills Network Cloud IDE environment, which provides access to a Linux terminal.

## Part 1: Windows tickets
- Add a new user to a new group
- Update and run virus and threat protection
- Configure firewall and network protection

## Part 2: Linux tickets
- Create a new user
- Manage files and folders
- Apply system updates

## Ticket 1: Create a new user
In this task, I will use Microsoft Windows Server Manager to create a new user and group and then add the user to the group.

- Open Server Manager
- Create a new user named after one of your favorite cartoon characters.
- Set a secure password.

![image](https://github.com/user-attachments/assets/5f59687c-05f6-4603-89b6-a6a0fec33902)

- Create a new group named Accounting.

![image](https://github.com/user-attachments/assets/421c7ad2-b5fb-4bab-91bb-81ef003d79c4)

## Ticket 2: Check for virus and threat protection updates
In this task, I will use the Windows operating system to check for virus and threat protection updates and run a "Quick Scan".

- Check for updates to virus and threat protection.  
![image](https://github.com/user-attachments/assets/67015439-3823-4430-86da-61bb5ca2bf1a)

- Run a Quick Scan using Windows Security.
![image](https://github.com/user-attachments/assets/a2e29437-bcb3-409a-9cfc-96a309a1c4af)

## Ticket 3: Configure firewall and network protection
Access Windows Defender Firewall with Advanced Security to create a new rule with following properties.
1.  A port rule that controls connections for a TCP port on port 80
2.  Allow the connection on Domain, Private, and Public.
3.  Includes the rule name: "Port 80 Permitted"
![image](https://github.com/user-attachments/assets/17220167-3a5f-405c-9d7f-2329543d5489)

## Ticket 4: Create a new user
- Create a new user with the adduser command and name the user after a favorite cartoon character.
- Set a secure password and complete other information prompted for.
- Display the newly created account using the command cat /etc/passwd | grep {username}.
![image](https://github.com/user-attachments/assets/f3ba8a3f-40a9-4e2b-a019-34d3e65ba928)

### Ticket 5: Manage files and folders
- Create folders named Accounting and Payroll
- Display the new folders and take a screenshot.
- Create a file named Best Practices inside the Accounting folder.
- Display the contents of the Accounting folder.
![image](https://github.com/user-attachments/assets/f7d613ed-9e10-48cc-ab52-6e39699b0b64)

## Ticket 6: Apply system updates
- Check for updates using the sudo apt update command.
- Use the sudo apt upgrade command to install updates.
![image](https://github.com/user-attachments/assets/50ada463-3fcc-4aaa-92d4-9787be390e21)
- Use the less /var/log/dpkg.log command to display a list of recent updates.
![image](https://github.com/user-attachments/assets/827b775e-0660-4458-9801-739b49567d3d)




