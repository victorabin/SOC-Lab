# SOC-Lab
SOC Lab Project – Creating a Home SOC Lab using Elastic SIEM.
I have recently completed a hands-on Security Operations Center lab project where I was able to create my own small SOC environment and learn how security monitoring and detection work.
# Lab Setup
The environment consisted of:
* Elastic Cloud SIEM for log ingestion and analysis
* Kibana for investigation and dashboard visualization
* Kali Linux Virtual Machine as the monitored endpoint
* Elastic Agent (Elastic Defend) for endpoint telemetry

# Implementation
##  Elastic Deployment
Created an Elastic Cloud deployment and launched Kibana to access security monitoring features.

## Endpoint Setup
Configured a Kali Linux VM and installed Elastic Agent to forward system and process logs to Elastic SIEM.

## Event Generation
Simulated security activity by running Nmap scans (nmap -T4 -A -v localhost) to generate observable security events such as port discovery and service enumeration.


## Log Investigation
Used Kibana Discover to query logs and analyze events using filters like:process.name:nmap

## Dashboard Creation
Created a custom dashboard to visualize Nmap-related events using timestamps and event counts.

## Alert Configuration
Configured a custom detection rule to trigger alerts when Nmap activity appears in logs.


# Key Takeaways
* SIEM deployment and configuration
* Endpoint log collection using Elastic Agent
* Log investigation using Kibana queries
* Security dashboard creation
* Detection rule and alert configuration


This project has helped me comprehend how endpoint log data is gathered, processed, and utilized in threat detection within a SOC environment.
