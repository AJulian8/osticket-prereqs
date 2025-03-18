# osticket-prereqs<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This project outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a virtual machine.
- Enable Internet Information Services (IIS)
- Install Web Platform Installer
- Install MySQL and set up username and password
- Finish installing osTicket
  

<h2>osTicket Lab</h2>

<p>
<img src="https://i.imgur.com/9yU8QgZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
So first things first I went and made a virtual machine in Microsft Azure and named it osTicket. I now want to copy the IP address so I can log into my virtual desktop and start the proccess of setting up osTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/kkIVG9p.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this example we have already extracted from a zip file and are now starting the process of setting up all the background necessities that osTicket needs to run properly. Here I am enabling IIS with CGI.
</p>
<br />

<p>
<img src="https://i.imgur.com/lwdUBDs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next from that same osTicket file we want to then install PHP manager.
</p>
<br />

<img src="https://i.imgur.com/r1u0zLj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here we installed the rewrite module and created a "PHP" folder on the C drive which we see opened in this image.
</p>
<br />

<img src="https://i.imgur.com/C4ilEAL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Wrapping up all the downloads from that extracted file we downloaded VC- Redist and MySQL changed it to a typical setup launched it and created our username and password. Now weve opened IIS as a admin and registered PHP from within IIS we then want to reload it to make sure everything worked properly.
</p>
<br />

<img src="https://i.imgur.com/J24S8JF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next we installed osTicket in the wwwroot folder on the C drive and changed the name of the file to osTicket.
</p>
<br />

<img src="https://i.imgur.com/7CzMHdw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
So after opening opening sites and then the osTicket folder in IIS manager we noticed we had some extentions that we needed to add. Which is what we see here the php_imap.dll,  php_intl.dll, and php_opcache.dll have been enabled.
</p>
<br />

<img src="https://i.imgur.com/ebMFwBT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this image we can see that majority of the osTicket installer page is checked, which is great! Now we just have a few more steps which are set up some permissions, name our helpdesk, and install HeidiSQL. After that well be able to sign in and use osTicket!
</p>
<br />

<img src="https://i.imgur.com/c4CwXRR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here we gave everyone full control on the permissions which would't be recommended for a secure business setup but for this intance it will work just fine.
</p>
<br />

<img src="https://i.imgur.com/JUYE9ZZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here we downloaded HeidiSQL and opened it created a session then connected to our session. We then created a database and named it osTicket and we can see that everything is there and good to go.
</p>
<br />

<img src="https://i.imgur.com/URXJWFO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
When you see this osTicket is set up correctly and good to go!
</p>
<br />

<img src="https://i.imgur.com/2qn4sNg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This is what osTicket will look like when you log in on the login page.
</p>
<br />

