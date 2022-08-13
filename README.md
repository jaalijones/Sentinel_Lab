<h1>Failed RDP to IP Geolocation Information</h1>

<h2>Description</h2>
<b>The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third party API to collect geographic information about the attackers location.
</b>
<br />
<br />
The script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot.
We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to
look up the attackers Geolocation information and plot it on an Azure Sentinel Map!
<br />
<br />

<p align="center">
<img src="https://user-images.githubusercontent.com/110305863/184516108-2c523e8d-fbc1-4124-a587-15247473396f.JPG" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks from China & Thailand coming in; Custom logs being output with geodata</h2>

<p align="center">
<img src="https://user-images.githubusercontent.com/110305863/184515685-23b54476-dce1-4fcb-954d-abbaae4a6492.JPG" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>World map of incoming attacks after 24 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://user-images.githubusercontent.com/110305863/184511488-4f80f9cf-3a13-4883-b513-5c126614bbee.JPG" height="85%" width="85%" alt="Image Analysis Dataflow"/>

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
