# Module 5 - Final Project

## Learning Objectives
- Design a network with subnets
- Configure Firewall Rules Using Microsoft Windows Defender Firewall
- Analyze HTTP/HTTPS Website Traffic for Using Wireshark
- Calculate Subnet Addresses and Subnet Masks

## Final Project Overview

In this final project you'll apply your skills to a real-life scenario where you help a company set up a new network. Based on what you’ve learned in this course. you'll provide detailed recommendations,  strategies, and justifications for the following network planning considerations:

- Design a network with subnets
- Calculate subnet addresses and subnet masks
- Analyze HTTP/HTTPS Traffic for one website using Wireshark
- Configure firewall rules using Microsoft Windows Defender  Firewall

## Final project requirements:
If you decide to try this poject on your own machine, you will need access to:

- A workstation running Microsoft Windows 10 or later
- Administrator rights to the workstation

## Scenario:
TechSafe, Ltd. has hired you to design and secure its network. The company uses a fixed IP address from its Internet service provider (ISP) and wants a structured network with compatible IP addressing, subnetting, and security configurations.

## Task 1: Design a network with subnets
Scenario: Design a network diagram for TechSafe Ltd that includes three departments: Administration, Sales, and IT. Each department requires its own subnet.
### Deliverable: A screenshot of the network diagram.
- One router connected to one switch. The router connects to the switch with a line. Label the router as Router and label the switch as Switch.
- Three subnets that connect to the switch using solid lines The three subnets are labeled as Administration, Sales, and IT.
- The diagram includes no additional elements beyond the router, switch, and subnets.

![Task1_NetworkDiagram](https://github.com/user-attachments/assets/f86db237-b353-402c-8144-66ca05f709fd)

## Task 2: Calculate Subnet Addresses and Subnet Masks
Scenario: You are working with a fixed IP address of 198.51.100.0/24. The network is divided into three subnets with the following IP address ranges for each department:
- Administration: 198.51.100.1 - 198.51.100.62
- Sales: 198.51.100.65 - 198.51.100.126
- IT: 198.51.100.129 - 198.51.100.190
Your task is to calculate each department's subnet addresses and subnet masks based on their specified IP address ranges and save that information into a text-based table for later use.

### Deliverable: A screenshot of the department subnet addresses, masks, and address ranges
Before capturing the screenshot, verify that your table displays the following information:
- Four columns: Subnet Name, Subnet Address, Subnet Mask, and IP Address Range. These labels are displayed at the top of each column.
- One row for each subnet (Administration, Sales, IT).
- Each subnet name's subnet address, mask, and IP address range.
- No additional text beyond the table.

![Task2Screenshot1](https://github.com/user-attachments/assets/8437d678-8a60-4084-a699-f66f98a2cfa2)

## Task 3: Analyze HTTP/HTTPS Website Traffic for Using Wireshark
Scenario: After implementing the network design in Task 1 and configuring the IP addresses and subnets during Task 2, TechSafe Ltd. needs you to monitor network usage related to website that their employees might access. Your task is to capture and analyze HTTP/HTTPS traffic from one of the following websites to identify and understand the data flow related to these two services.

### Deliverables: Submit one screenshots of your Wireshark analysis:
Screenshot of the Wireshark application displaying filtered traffic.

![Task3Screenshot1](https://github.com/user-attachments/assets/e448a1a3-5f2c-49a0-afa2-84c809568cb5)

## Task 4: Configure Firewall Rules Using Microsoft Windows Defender Firewall
Scenario: TechSafe Ltd. wants to further secure its internal network by restricting access to specific types of web traffic. To enhance security, you must go to each workstation and configure Microsoft Windows Defender Firewall to block all FTP and HTTP traffic.

### Steps
- Open a terminal window and type  ftp ftp.dlptest.com
- Capture a screenshot that shows successful access to ftp ftp.dlptest.com before applying the firewall rule.

![Task4Screenshot1](https://github.com/user-attachments/assets/09e01b64-d9b4-4f0b-a75b-5b32f1e2106d)

- Open Microsoft Windows Defender Firewall and access its advanced settings to create a new custom outbound rule to block all FTP traffic (Port 21).

![Task4Screenshot2](https://github.com/user-attachments/assets/49b52cbe-0b3c-4267-a0a4-d093d1410fef)

- Verify that the rule to block FTP access is working. Open a terminal window and again type ftp ftp.dlptest.com to confirm that access is blocked.

![Task4Screenshot3](https://github.com/user-attachments/assets/bae6cc7c-0d2b-4b21-a7eb-0738ff28886d)

- Open a browser and access http://httpforever.com/. If you see a cautionary message that this website is not secured, select the onscreen message that enables you to proceed to the site.

![Task4Screenshot4](https://github.com/user-attachments/assets/3eac9042-232f-4795-95c2-b2d4e2ea6419)

- Open Windows Defender Firewall and access the advanced settings to create a new custom outbound rule to block all HTTP traffic (Port 80).

![Task4Screenshot5](https://github.com/user-attachments/assets/b1239e3a-a68b-4793-a621-6bb00972e2cb)

- Verify that the HTTP traffic is active and correctly configured within your firewall settings by attempting to access http://httpforever.com/.

![Task4Screenshot6](https://github.com/user-attachments/assets/feaa85b8-96bd-4e4f-9c77-969d5c596cae)

