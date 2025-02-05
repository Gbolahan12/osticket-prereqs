# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- PHP Manager
- Rewrite Module
- VC_redist.x86.exe
- MySQL
- HediSQL

<h2>Installation Steps</h2>

<p>
  
<img src="https://i.imgur.com/s954qSU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p></p>
  <img src="https://i.imgur.com/EX4i8uR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate to Microsoft Azure and create a resource group
</p>

<br />

<p>
<img src="https://i.imgur.com/P4GveBv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once my resource group is created, next I'll create the virtual machine.
</p>
<p>
<img src="https://i.imgur.com/1NArKMR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/2VhtM6b.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<p>
<img src="https://i.imgur.com/jZ1YPci.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  <p>
<img src="https://i.imgur.com/tbu9tOu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    
Now I am done setting up my virtual machine.
</p>
<p>
<img src="https://i.imgur.com/MPp38av.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  Once it has been created I'll use Remote Desktop Connection to connect to the virtual machine.
</p>
<p>
<img src="https://i.imgur.com/2F8btZb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  <p>
    <img src="https://i.imgur.com/7523QOe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  </p>
  
I will install and enable IIS (Internet Information Servies) by going to Control Panel> Programs> Turn Windows Features On or Off> Internet Information Services and enable it then World Wide Web Services> Application Development Features and enable CGI
</p>

<img src="https://i.imgur.com/3OpE8ib.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
Now I will install PHP manager to setup my IIS.

</p>

</p>
<img src="https://i.imgur.com/INir68n.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
I will also install Rewrite Module.
</p>

</p>
<img src="https://i.imgur.com/Spsvrir.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
Then I will create a PHP directory on the C drive.
</p>

</p>
<img src="https://i.imgur.com/Ykv576W.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
Now I'll open the zipped PHP folder and extract the file in the PHP directory I just made
</p>

</p>
<img src="https://i.imgur.com/JMTM04O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
I will then install Microsoft Visual C++
</p>

</p>
<img src="https://i.imgur.com/ffC8T3x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
Now I install MySQL and go through the installation settings.
</p>

<br />
