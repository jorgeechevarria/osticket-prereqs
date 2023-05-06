<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This overview tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket. osTicket is a widely-used open-source ticketing system that allows businesses and organizations to manage and track customer support requests from a single platform. It provides a user-friendly interface for both customers and support agents, allowing for efficient communication and ticket resolution.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Creating azure enviroment
- PHP manager for IIS
- rewrite module
- create directory c:\PHP
- c++ Redistributable
- MySQL server database

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/cPgOydz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First step is to create the enviroment where osTicket will be. on Azure make a resource group, and create a virtual machine. when making a VM (virtual machine) azure creates a virtual network, on the image is the Resource group created, virtual machine and, virtual network. (note: login to your VM with IP in remote desktop and use the user created in azure for VM )
</p>
<br />

<p>
<img src="https://i.imgur.com/kH1sAoC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search and run IIS as an administrator. (to do that hover over IIS, right click.) when opens, select the icon "PHP Manager". when inside, select
  "register new php version " in the next images provided take a closer look of the whole process to register new php. ( note: refresh IIS when done. )
</p>
<br />

<p>
<img src="https://i.imgur.com/a7VfpaP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
.
</p>
<br />
