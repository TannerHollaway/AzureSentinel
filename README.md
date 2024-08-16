<h2>Creating a honeynet in Azure</h2>
I am thrilled to present my latest project, which focuses on building a honeynet in Azure to simulate real-world cyber attacks. This project showcases my skills in Azure security, incident response, and environment hardening
<br />

<h2>Objective</h2>

The main objective of this project was to set up [virtual machines](https://github.com/TannerHollaway/VirtualMachineCreation) that were intentionally vulnerable in the Azure infrastructure to attract and analyze cyber attacks. This helped me to better understand the tactics and techniques used by attackers, while also showcasing my ability to respond quickly and effectively to any identified issues.
<br />




<h2>Utilities Used</h2>

- <b>Azure Virtual Network (VNet)</b> 
- <b>Azure Network Security Group (NSG)</b>
- <b>Virtual Machines (2x Windows, 1x Linux)</b>
- <b>Log Analytics Workspace with Kusto Query Language (KQL) Queries</b>
- <b>Azure Key Vault for Secure Secrets Management</b>
- <b>Azure Storage Account for Data Storage</b>
- <b>Microsoft Sentinel for Security Information and Event Management (SIEM)</b>
- <b>Microsoft Defender for Cloud to Protect Cloud Resources</b>
- <b>Windows Remote Desktop for Remote Access</b>
- <b>Command Line Interface (CLI) for System Management</b>
- <b>PowerShell for Automation and Configuration Management</b>
- <b>PowerShell for Automation and Configuration Management</b>
- <b>NIST SP 800-61 Revision 2 for Incident Handling Guidance


<h2>Methodology:</h2>

<b>Creating the honeynet: I began by deploying multiple vulnerable [virtual machines](https://github.com/TannerHollaway/VirtualMachineCreation) in Azure, simulating an secure envoriment</b>


<h2>Monitoring and analysis:</h2>

Azure was configured to ingest log sources from various resources into a log analytics workspace. Microsoft Sentinel was then used to build attack maps, trigger alerts, and create incidents based on the collected data.



<h2>Security metrics measurement:</h2>
<p align="center">
I observed the environment for around 4 to 5 hours, recording key security metrics while it was insecure. This provided a baseline to compare against after implementing remediation measures.
<br/> 
<img src="https://github.com/user-attachments/assets/f8be990a-09dc-4ec7-b660-0390c4d6127d" height="80%" width="80%" alt="NSGALLOW"/>
<br />
<br />
<p align="center">
<img src="https://github.com/user-attachments/assets/dced1de9-3642-41ae-961e-f8074966c82f" height="80%" width="80%" alt="RDPfail"/>


<h2>Incident response and remediation:</h2>

After addressing the incidents and identifying vulnerabilities, I began the process of hardening the environment by applying security best practices and Azure-specific recommendations. You can see the strengthening of the environment [here](https://github.com/TannerHollaway/Becoming-NIST-80053-compliant) And my incident response Labs [here](https://github.com/TannerHollaway/Incident-Response)


<h2>Post-remediation analysis:</h2>

I re-observed the environment for another 5to 6 hours to measure security metrics again, comparing the results with the initial baseline. Unfortunately heatmaps don't work when there are no alerts or logs to ingest.
- Metrics before hardening and Security control implimentation.
  
| **Metric**                          | **Count** |
|--------------------------------------|-----------|
| SecurityEvent (Windows VM)           | 15,355   |
| SecurityAlert (Microsoft Defender for Cloud) | 20     |
| SecurityIncident (Sentinel Incidents) | 23       |
| NSG Inbound Malicious Flows Allowed  | 1697       |

- Metrics after hardening and security control implimentation
  
| **Metric**                          | **Count** |
|--------------------------------------|-----------|
| SecurityEvent (Windows VM)           | 2980   |
| SecurityAlert (Microsoft Defender for Cloud) | 0     |
| SecurityIncident (Sentinel Incidents) | 0       |
| NSG Inbound Malicious Flows Allowed  | 0       |

<h2>Conclusion</h2>

To conclude, I successfully established a compact yet powerful honeynet using Microsoft Azure's robust cloud infrastructure. Microsoft Sentinel was employed to generate alerts and incidents based on the logs collected from the configured watch lists. Initially, baseline metrics were recorded in the unprotected environment before any security controls were implemented. Following this, a series of security measures were put in place to strengthen the network against potential threats. After these controls were applied, a second set of measurements was conducted.

The comparison between the pre- and post-implementation metrics revealed a substantial decrease in security events and incidents, underscoring the effectiveness of the implemented security controls. It's worth noting that if the network's resources had been heavily utilized by regular users, or I left them on for longer periods of time, it is highly likely that a greater number of security events and alerts could have been observed within the 24-hour period following the implementation of these security controls.






