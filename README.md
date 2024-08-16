<h2>Creating a honeynet in Azure</h2>
I am thrilled to present my latest project, which focuses on building a honeynet in Azure to simulate real-world cyber attacks. This project showcases my skills in Azure security, incident response, and environment hardening
<br />

<h2>Objective</h2>
The main objective of this project was to set up virtual machines that were intentionally vulnerable in the Azure infrastructure to attract and analyze cyber attacks. This helped me to better understand the tactics and techniques used by attackers, while also showcasing my ability to respond quickly and effectively to any identified issues.
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
Creating the honeynet: I began by deploying multiple vulnerable [virtual machines](https://github.com/TannerHollaway/VirtualMachineCreation) in Azure, simulating an insecure environment.

<h2>Monitoring and analysis::</h2>
Azure was configured to ingest log sources from various resources into a log analytics workspace. Microsoft Sentinel was then used to build attack maps, trigger alerts, and create incidents based on the collected data.

<h2>Security metrics measurement:</h2>
<p align="center">
I observed the environment for around 4 to 5 hours, recording key security metrics while it was insecure. This provided a baseline to compare against after implementing remediation measures.
<br/> 
<img src="https://github.com/user-attachments/assets/f8be990a-09dc-4ec7-b660-0390c4d6127d" height="80%" width="80%" alt="NSGALLOW"/>
<br />
<br />





<p align="center">
ExampleTextForScreenshot <br/> 
<img src="ExampleScreenshot" height="80%" width="80%" alt="ScreenshotName"/>
<br />
<br />


<p align="center">
ExampleTextForScreenshot <br/> 
<img src="ExampleScreenshot" height="80%" width="80%" alt="ScreenshotName"/>
<br />
<br />


<p align="center">
ExampleTextForScreenshot <br/> 
<img src="ExampleScreenshot" height="80%" width="80%" alt="ScreenshotName"/>
<br />
<br />


<p align="center">
ExampleTextForScreenshot <br/> 
<img src="ExampleScreenshot" height="80%" width="80%" alt="ScreenshotName"/>
<br />
<br />


<p align="center">
ExampleTextForScreenshot <br/> 
<img src="ExampleScreenshot" height="80%" width="80%" alt="ScreenshotName"/>
<br />
<br />


<p align="center">
ExampleTextForScreenshot <br/> 
<img src="ExampleScreenshot" height="80%" width="80%" alt="ScreenshotName"/>
<br />
<br />


<p align="center">
ExampleTextForScreenshot <br/> 
<img src="ExampleScreenshot" height="80%" width="80%" alt="ScreenshotName"/>
<br />
<br />

