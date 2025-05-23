# Module 4 - 

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
