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

## Task 3: Analyze HTTP/HTTPS Website Traffic for Using Wireshark
Scenario: After implementing the network design in Task 1 and configuring the IP addresses and subnets during Task 2, TechSafe Ltd. needs you to monitor network usage related to website that their employees might access. Your task is to capture and analyze HTTP/HTTPS traffic from one of the following websites to identify and understand the data flow related to these two services.

### Deliverables: Submit one screenshots of your Wireshark analysis:
Screenshot of the Wireshark application displaying filtered traffic.
