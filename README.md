<h1>Build An Elastic SIEM </h1>

<h2>Description</h2>
Project consists of simple walk through steps on how to set up a home lab for Elastic Stack Security Information and Event Management (SIEM) using the Elastic Web portal and a Kali Linux VM. You will also learn how to generate security events on the Kali VM, set up an agent to forward data to the SIEM, and query and analyze the logs in the SIEM.

<br />


<h2>Operating System Used<h2>

- <b>MacOS Monterey Version 12.7.4</b>

<h2>Downloads<h2>
 
- <b>VirtualBox 7.0.14</b>
- <b>Kali Linux VM</b>
- <b>Elastic account</b>

<h2>Project walk-through:</h2>

<p align="center">
Download VirtualBox: <br/>
<img src="https://i.imgur.com/TrQnZkK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Download Kali Linux: <br/>
<img src="https://i.imgur.com/M6gccC7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Using '+' add Kali Linux download to VirtualBox: <br/>
<img src="https://i.imgur.com/eoJHcJ9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
With "Start" launch Kali Box:  <br/>
<img src="https://i.imgur.com/E0s7KwZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Log into Elastic SIEM -> Navigate to 'Integrations' -> Download "Elastic Defend":  <br/>
<img src="https://i.imgur.com/BXmTwTc.png)height=" height=80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Paste command into Kali Terminal -> "ENTER" for install:  <br/>
<img src="https://i.imgur.com/NyjiXmG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once message “Elastic Agent has been successfully installed.” It will automatically start collecting and forwarding logs to your Elastic SIEM  <br/>
<img src="https://i.imgur.com/AW19rNt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Verify that the agent has been installed correctly by running this command: sudo systemctl status elastic-agent.service  <br/>
<img src="https://i.imgur.com/BSbRH5o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Security Events by using "Nmap" (“nmap -sS <ip address>”, “nmap -sT <ip address>”, “nmap -p- <ip address>”etc..) <br/>
<img src="https://i.imgur.com/zCVJzfU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Navigate to "Logs" in Elastic to view logs fron Kali VM  <br/>
<img src="https://i.imgur.com/aj1TnOD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Filter the results by using "Search"  <br/>
<img src="https://i.imgur.com/byjLPJn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once message “Elastic Agent has been successfully installed.” It will automatically start collecting and forwarding logs to your Elastic SIEM  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
