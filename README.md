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
<img src="https://i.imgur.com/fFSOHCQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <p>
    <img src="https://i.imgur.com/ffC8T3x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  </p>
    <p>
    <img src="https://i.imgur.com/vzl1bTL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  </p>
  <p>
    <img src="https://i.imgur.com/1Sqs2tj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  </p>
Now I install MySQL and go through the installation settings.
</p>

 <p>
    <img src="https://i.imgur.com/hgtqRFa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  </p>

  <p>
    <img src="https://i.imgur.com/8mdB70Z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  </p>

  <p>
    <img src="https://i.imgur.com/hFQ82iW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  </p>
  
I open IIS as an Administrator go to PHP Manager> Register new PHP version and then select the file shown.

<p>
    <img src="https://i.imgur.com/G85S8tI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  </p>

  <p>
    <img src="https://i.imgur.com/tMsvUn0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    
  Next I'll unzip osTicket folder and copy the "upload" file to the wwwroot file in the inetpub directory, Rename "upload" folder to "osTicket".
  </p>

  
   <p>
   <img src="https://i.imgur.com/jDFzzMt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
    <img src="https://i.imgur.com/k3iLDw4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
 
Now open IIS and load the Browser *80 Notice some extensions are not enabled. I'll enable a few of those in IIS. Go to Sites> Default Web Site> osTicket Click PHP Manager> Enable or disable an extension. Enable php_imap.dll, php_intl.dll, and php_opcache.dll.
  </p>

<p>
    <img src="https://i.imgur.com/yYjBxUp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Next browse in file explorer to C drive> osTicket> include> ost-sampleconfig.php and remove the "sample" from the name.

</p>

<p>
    <img src="https://i.imgur.com/flhTzKy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>

<p>
    <img src="https://i.imgur.com/VCMrFjI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

I will right-click on ost-config.php> Properties> Security> Advanced> Disable Inheritance> Remove all inherited permissions from this object, Click on the add buton to add permissions to the file> Select a principle> type "everyone"> Check Names> OK> check all permissions> OK> apply> OK.

</p>

<p>
    <img src="https://i.imgur.com/2RDH95f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Go back to the browser and hit continue on the osTicket webpage and fill out the setup page.

</p>

<p>
    <img src="https://i.imgur.com/llb8gHn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
      <img src="https://i.imgur.com/qgwQU0A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>

<p>
        <img src="https://i.imgur.com/qINfpvU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Install HediSQL for out database setup.
we'll have to connect the database using HeidiSQL, In HeidiSQL click New> Username = root> Password = root > open. 

</p>

</p>
<p>
        <img src="https://i.imgur.com/hJQgAS9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>

  <img src="https://i.imgur.com/eKG4sK1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
</p>
Go to the browser reload the webpage and Observe the changes. CONGRATULATIONS!

</p>

<br />

<h2>osTicket Installed!</h2>

<b>osTicket is now installed and ready for use! In the next project I will walk you through how to configure agents, their permissions and access, users, and more!  </b>
<br />
<br />
</p>
