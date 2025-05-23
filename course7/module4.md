# Module 4 - Detection and Response
In this module, you will learn about detecting cyberattacks and responding to them. This module will introduce you to security being the sum of prevention, detection, and response. You will be introduced to detection using the security information and event management (SIEM) system or extended detection response (XDR) system detection techniques to perform tasks such as monitoring, analyzing, reporting, and threat hunting. You will also get an overview of the SIEM process followed by the XDR process and how SIEM and XDR work together. Further, you will be introduced to federated search. This module will also cover how to respond to cyberattacks. You will become familiar with the SOAR system and also understand how automation and orchestration differ. Finally, you will be introduced to breach notifications.

## Detection
The CIA triad represents the What of cybersecurity and shows what we are trying to do with cybersecurity.

Security is about Prevention, Detection, and Response (S = P + D + R). This represents the How of the security.

Detection is about receiving information from all the domains and feed them into a monitoring engine. This is followed by analyzing, reporting, and threat hunting.

Detection and Response activities are performed by the Security Operations Center (SOC) team within an organization.

Types of detection technologies
Technologies used to do this kind of work include:

- Security Information and Event Management (SIEM)
- Extended Detection and Response (XDR)

## Security Information and Event Management (SIEM)
### Need for SIEM
Having individual security consoles for each domain with specialized cybersecurity analysts for each domain can be expensive. Further, there is no way to get a single consistent view of all the domains. If an attacker breaks one system, there may be alarms on different domain consoles, which can result in several people trying to solve the same problem, which is inefficient.

This is why the SIEM system came into existence.

### Functioning of SIEM systems
It is necessary to reduce the footprint and provide a single point that gives you the visibility of all the systems, gather all the information, and bring it up through the analysis.
With SIEM, a new layer is added at the top of all system consoles. Let's look at the different steps involved once the SIEM layer is added.

- Collect information, such as logs, alarms, events, and flow data, from each domain's security consoles. This information is stored in a database.
- Next, apply analytics to it. Correlate the information and get it down into a manageable subset.
- Then, you will need to analyze the information. To do this, you can:
- Leverage the rules set up in the SIEM system or customize the rules to adhere to the policies. Based on the results, the priorities for notifications and actions are set as High, Medium, and Low.
- Look for anomalies. Examples of anomalies are any specific use cases or specific indicators of compromise. Using Artificial Intelligence (AI), specifically Machine Learning (ML), to determine patterns will be very useful in this situation.
Note: The technology used to find and analyze anomalies is referred to as User Behavior Analytics (UBA).
- Finally, review the reports to understand the trends. The reports help the SOC team answer questions, such as:

- Are we doing better now than earlier?
- Are we resolving faster?

## Extended Detection and Response system (XDR)
With Endpoint Detection and Response (EDR), an agent is installed on each system for detection along with a certain level of response. XDR was developed to read and hold all the information from the EDR or SIEM and some vendors added the capability of federated search to look for particular indicators of compromise across all systems. The advantage is that there is no need for prefetched data in a database. You can get information just in time. A federated search tells the systems to fetch the data just in time.

### SIEM and XDR
SIEM uses a bottom-up approach, while XDR uses a top-down approach.
SIEM is good at triggering alarms, and an alarm from SIEM to XDR may be a good place to start an investigation.
Important: XDR plus SIEM can complement each other and make a stronger security response. They help monitor, analyze, and report on all activities happening in the environment.

## Threat hunting
It is important to detect an attack as soon as possible. This is done with threat hunting.

Threat hunting is a proactive initiative for an organization. This is where a cybersecurity analyst with experience and a good instinct can help with a hypothesis based on which we can determine the tools to detect threats or possible attacks, which results in early detection.

# Responding to an Attack
A good incident response can cut the cost of a data breach.

Traditionally, an attack is referred to as an incident, and the response is an incident response (IR). An IR is typically resolved by an expert manually. The expert will triage and remediate the incident.

In the modern world, with a focus on shortening the MTTC, you can use the Security Orchestration, Automation and Response (SOAR) technology. The focus of SOAR is on automating as much of the IR process as possible.

## Cases
- When an attack generates an alarm, The SIEM or the XDR system will initiate a case in the case management component of the SOAR system.
- Next, assign the case to the appropriate cybersecurity analyst.
- The analyst then investigates the incident. To ensure that the process is consistent and repeatable, the analyst can use the dynamic playbook.
- The dynamic playbook provides a set of steps based on an algorithm to enable the analyst to perform the investigation activities.
- Once the analyst determines the cause and remediation steps, action to remediate the system can be applied.

## Automation and Orchestration
While automation is a great practice, not everything can be automated because there are several first-of-a-kind (FOAK) events.

- Automate what you can.
- Orchestrate wherever automation is not possible.
- Breach Notification

In case of a breach, you will need to:
- Determine the data sets that are impacted.
- Determine the geographic location where the data was breached.
- Inform the regulatory body in the location.

IMPORTANT: You will pay a penalty if you do not notify the regulatory body in the location.
