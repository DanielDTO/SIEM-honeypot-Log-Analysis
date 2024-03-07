<h1>SIEM Honeypot IP Geolocation Analysis</h1>

<h2>DESCRIPTION</h2>
<b>The project focuses on collecting login data from a Windows host machine. A powershell script running on the machine, is responsible for parsing out Windows Event Log information for failed RDP attacks and with a third party API, it collects geographic information about the attackers location.
</b>
<br />
<br />
Azure Sentinel (SIEM) is used and is connected to a live virtual machine which is the honeypot in this experiment. Using Sentinel, live RDP brute force attacks are observed from all over the world. A custom PowerShell script is used to look up the attackers Geolocation information and plot it on an Azure Sentinel Map!
<br />
<br />

<p align="center">
<img src="https://github.com/DanielDTO/SIEM-honeypot-project/assets/22667819/8529de61-6c0d-4258-9f44-b86f1cdb3dfc" height="80%" width="80%" alt="RDP fail logs to IP Geolocation"/>
</p>

<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API
- <b>Microsoft Azure:</b> Virtual Machine (honeypot) creation, Log Analytics Workspace, Sentinel, Custom Log creation

<h2>World Map of Incoming attacks from around the World over 4 days (Custom logs being output with geodata)</h2>

<p align="center">
<img src="https://github.com/DanielDTO/SIEM-honeypot-project/assets/22667819/fee92f37-a373-4aa5-8142-3640c16d6a44" height="80%" width="80%" alt="RDP fail logs to IP Geolocation"/>
</p>


<p align="center">
<img src="https://github.com/DanielDTO/SIEM-honeypot-project/assets/22667819/f38b4b0f-2b6d-498a-b151-2b58f0492d97" height="80%" width="80%" alt="RDP fail logs to IP Geolocation"/>
</p>


<p align="center">
<img src="https://github.com/DanielDTO/SIEM-honeypot-project/assets/22667819/b41158e3-995a-443d-8196-b56b5414f9f5" height="80%" width="80%" alt="RDP fail logs to IP Geolocation"/>
</p>

<p align="center">
<img src="https://github.com/DanielDTO/SIEM-honeypot-project/assets/22667819/e61c8350-2c1c-4fc9-b625-18aa90049cbb" height="80%" width="80%" alt="RDP fail logs to IP Geolocation"/>
</p>
