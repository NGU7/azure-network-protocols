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
<img width="1440" alt="Screen Shot 2025-01-22 at 5 59 48 PM" src="https://github.com/user-attachments/assets/06e4fb4e-8616-42f1-9885-ea815c8e0626" />

</p>
<p>
Once the prerequisites are complete the web server will display green checkmarks allowing you to continue into the ticketing system. From here we create the name of our help desk as well as our admin overseer to manage our ticketing system.
</p>
<br />

<p>
  <img width="1440" alt="Successful OsTicket Login" src="https://github.com/user-attachments/assets/fb37f7e7-64ec-410a-9897-cf01729d7992" />
</p>
<p>
  After a successful installation and login, the first panel you access is the ticketing panel where all end-user and agents' current tickets will be displayed.
</p>
<br />
