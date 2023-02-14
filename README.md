<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- While aleady in your MS Azure account, create a resource group 
- Create a Windows 10 Virtual Machine (VM) with 2-4 virtual CPUs, when creating the vm, allow it to create a new Virtual Network (Vnet).
You can use these name for this tutorial or you change to whatever you want:
-Name: Vm-osticket
-Username: labuser (for example/whatever you chose)
-Password: osTicketPassword1! (for example/whatever you chose)

<h2>Installation Steps</h2>
-Step 1: Download and install PHP manager for IIS

-Step 2: Download and install Rewrite module

-Create and install directory C:\PHP
-Download PHP 7.3.8 and unzip the content into C:\PHP
-Download and install VC_redist.x.86.exe.
Download and install MySQL5.5.62
Typical Setup ->
- Launch Configuration Wizard (after install) ->
- Standard Configuration ->
- Password1

Register PHP from within IIS
Reload IIS (Open IIS, Stop and Start the server)
Install osTicket v1.15.8
- Download osTicket from the Installation Files Folder
- Extract and copy “upload” folder to c:\inetpub\wwwroot
- Within c:\inetpub\wwwroot, Rename “upload” to “osTicket
- Open IIS as an Admin
-Register PHP from within IIS

<p>
<img src="https://i.imgur.com/8mBa0iA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />
