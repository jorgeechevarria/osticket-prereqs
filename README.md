<p align="center">
<img src="https://i.imgur.com/8cy7Rzc.png" alt="osTicket logo"/>
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
Now to after downloading osTicket zip, drag upload file to wwwroot to extract. after extraction is completed rename "upload" to "osTicket". refresh IIS.
  in the next images are the visuals to this step.
  
</p>
<br />
<img src="https://i.imgur.com/gY94MS4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After refreshing go to ( IIS > sites > default > osticket ) than open up "browse *:80" also notice on the page you can see a few disabled extensions with Xs, visuals are below.
</p>
<p>
  
<img src="https://i.imgur.com/NN975uP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  
  Now lets enable a few of the extensions, on IIS go to osTicket and go to "PHP Manager" and click on " enable or disable an extension\ add extension"
  and enable this extensions "PHP_Imap.dll, PHP_intl.dll, PHP_opcache.dll". refresh website to see the enabled extensions, visuals are below.
</p>
<p>
  
<img src="https://i.imgur.com/a7JXMp1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  On "file explorer" rename "Ost-sampleconfig.php" to "Ost-config.php" than add permissions to "Ost-config.php" using right right click going to security and advanced, than remove all set by default permissions, add write "everyone" on white empty box. than select full control, click apply and ok. images below.
  
</p>
<p>
  
<img src="https://i.imgur.com/wLM0esc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>  
  
  </p>
<p>
  
<img src="https://i.imgur.com/uMbqidd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>  
  
<img src="https://i.imgur.com/sXq4baz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>  
  
On osticket in browser click "continue" fill in the credentials for you account, do not click "install now" yet! images below.

</p>
<p>  
  
<img src="https://i.imgur.com/R5kuYyV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>  
  
  After installing HeidiSQL, open HeidiSQL and create new, login with your 'ROOT' username. and create a new database inside HeidiSQL and name this database osTicket, right click on "Unnamed", create new, database. name it osTicket. images down below. 
  
</p>
<p>  
  
<img src="https://i.imgur.com/OBtxeqU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>  
  
 Going back to the credentials page on the browser, fill in "mySQL database" and put osTicket this is the folder created in HeidiSQL. use your root username and password on the page and, click install now. you should see a congratulation page also meaning it worked! images down below.
  
</p>
<p>  
  
<img src="https://i.imgur.com/iHjZId4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>  
  
 You are done! login to your osTicket.
  
  </p>
<p>  
  
<img src="https://i.imgur.com/lN4WvuS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
  
  Thank you for taking the time to look into this overview tutoria! 
