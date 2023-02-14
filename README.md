<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>[Video Demonstration](https://screenrec.com/share/E1quSIx7Cm)</h2>

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
Step 1: Install / Enable IIS in Windows WITH CGI

Step 2: Download and install PHP manager for IIS

Step 3: Download and install Rewrite module

Step 4: Create and install directory C:\PHP

Step 5: Download PHP 7.3.8 and unzip the content into C:\PHP

Step 6: Download and install VC_redist.x.86.exe.

Step 7: Download and install MySQL5.5.62
Typical Setup ->
- Launch Configuration Wizard (after install) ->
- Standard Configuration ->
- Password1

Step 8: Open IIS as an Admin
Register PHP from within IIS
Reload IIS (Open IIS, Stop and Start the server or restart)
Install osTicket v1.15.8
- Download osTicket from the Installation Files Folder
- Extract and copy “upload” folder to c:\inetpub\wwwroot
- Within c:\inetpub\wwwroot, Rename “upload” to “osTicket

Reload IIS (Open IIS, Stop and Start the server)
Go to sites -> Default -> osTicket
- On the right, click “Browse *:80”

Step:9 Enable the following:
Go back to IIS, sites -> Default -> osTicket
- Double-click PHP Manager
- Click “Enable or disable an extension”
- Enable: php_imap.dll
- Enable: php_intl.dll
- Enable: php_opcache.dll
- Refresh the osTicket site in your browse, observe the changes

Step 10: Rename: ost-config.php and assign permissions
- From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
- To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

-Assign Permissions: ost-config.php

Continue Setting up osTicket in the browser (click Continue)

Step 11: Download and install heidiSQL


Continue Setting up osticket in the browser


Congratulations, hopefully it is installed with no errors!

Last step- Step 12: Clean up
- Delete: C:\inetpub\wwwroot\osTicket\setup
- Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php

Now you can sign into the osTicket.

