<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Installation of all the Prerequisites of osTicket
- Confirming all the prerequisites on the osTicket Web Server
- Create an admin account 
- Access osTicket

<h2>Actions and Observations</h2>

<p>
<img width="1440" alt="ICMP PING CONNECTION TEST" src="https://github.com/user-attachments/assets/7e5956a3-aa85-458b-a795-df58906f385e" />
</p>
<p>
  Using the PING command in Windows Powershell to communicate between a Windows PC and a Mac to test if both are on the same network(They are). The app Wireshark in the back is used to track the specific TCP port used for the PING command.
</p>
<br />

<p>
<img width="1440" alt="CONFIGURE FIREWALL AGINST ICMP" src="https://github.com/user-attachments/assets/ace62640-f394-4895-a833-82ab9d768961" />
</p>
<p>
Configured the firewall of the Mac to deny ICMPv4 data to test altering the firewall and to test blocking specific unwanted information.
</p>
<br />

<p>
<img width="1440" alt="DHCP TRAFFIC THROU RENEW PUBLIC IP ADDRESS" src="https://github.com/user-attachments/assets/dda1da7f-4dcb-46bc-b7f1-56ca4e738dde" />
</p>
<p>
This test was to track DHCP information coming in and out of the Windows PC. Through the command IPCONFIG /RENEW it allowed for the public IP address to get readministered. Wireshark allows us to see traffic between the pc and the DHCP Server.
</p>
<br />
<p>
<img width="1440" alt="DNS TRAFFIC SEARCHING THROUGH INTERWEBS" src="https://github.com/user-attachments/assets/9d8ac49f-3e7b-4a19-8970-b443d86954ed" />
</p>
<p>
 This test allows us to see our DNS Traffic. In Powershell, we look up an example website like Google.com, where we then see all the traffic on the backend through Wireshark of how information is received and sent.
</p>
<br />
<p>
<img width="1440" alt="TCP PORT 3389 TRAFFIC OR Remote PC Traffic " src="https://github.com/user-attachments/assets/97d6a81c-3e09-4fd7-9f29-81536acf2619" />
</p>
<p>
And lastly, we check for TCP port 3389 or the Remote Desktop Protocol (RDP) connection. This connection monitors all the movements made on the computer through Remote Desktop whether it's typing or moving the mouse all that goes through TCP port 3389 which displays thousands of bits of data at a time as can be seen on the left.
</p>
<br />
