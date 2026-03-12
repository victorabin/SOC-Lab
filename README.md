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
<img width="1910" height="873" alt="1" src="https://github.com/user-attachments/assets/c9ab1529-4ffb-411b-b1ef-e0163485ac35" />
<img width="1907" height="878" alt="2" src="https://github.com/user-attachments/assets/4b45cc54-f07b-480c-b52a-706e09c43787" />

## Endpoint Setup
Configured a Kali Linux VM and installed Elastic Agent to forward system and process logs to Elastic SIEM.

## Event Generation
Simulated security activity by running Nmap scans (nmap -T4 -A -v localhost) to generate observable security events such as port discovery and service enumeration.
<img width="1920" height="945" alt="6" src="https://github.com/user-attachments/assets/ed8c5ab6-34b7-4ac9-9b70-8f3930844047" />

## Log Investigation
Used Kibana Discover to query logs and analyze events using filters like:process.name:nmap
<img width="1920" height="945" alt="5" src="https://github.com/user-attachments/assets/597b78ad-4739-47e6-a8e9-eb3ade372d50" />
<img width="1920" height="945" alt="7" src="https://github.com/user-attachments/assets/ca1d9667-7614-421f-b252-7da0ab5393ba" />


## Dashboard Creation
Created a custom dashboard to visualize Nmap-related events using timestamps and event counts.
<img width="1920" height="945" alt="8" src="https://github.com/user-attachments/assets/8a7f8fc3-adc6-4982-ab22-388028996bc8" />

## Alert Configuration
Configured a custom detection rule to trigger alerts when Nmap activity appears in logs.
<img width="1421" height="762" alt="10" src="https://github.com/user-attachments/assets/23aabc63-4d2c-4f06-9906-6d47b2c8f37f" />


# Key Takeaways
* SIEM deployment and configuration
* Endpoint log collection using Elastic Agent
* Log investigation using Kibana queries
* Security dashboard creation
* Detection rule and alert configuration


This project has helped me comprehend how endpoint log data is gathered, processed, and utilized in threat detection within a SOC environment.
