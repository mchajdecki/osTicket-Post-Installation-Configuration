# osTicket-Post-Installation-Configuration
Post Installation Set up of osTicket

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post Installation Configuration</h1>
This tutorial outlines the Post Installation Configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: osTicket Post Installation Configuration](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h1>This tutorial is a follow up to the previous <a href="https://github.com/mchajdecki/osticket-prerequisites-and-installation">os Ticket - Prerequisites and Installation </a></h1>

- The resources used in this osTicket Post Installation Configuration continue from the previous tutorial the - osTicket - Prerequisites and Installation.
- Log into the osTicket Windows Virtual Machine to continue.

<h2>Once the osTicket is installed there will be two ways to access the portal</h2>

- Admin/Analyst Login Page: <a href="http://localhost/osTicket/scp/login.php">Admin/Analyst Login</a> where you configure settings on the back end for osTicket.
- End Users osTicket URL: <a href="http://localhost/osTicket"> End Users osTicket URL</a> essentially a help desk worker that works on tickets.</a> 

<h3>In this tutorial we will access both portals the Admin and the End user for guidance and further configuration in osTicket , the open-source help desk system that centralizes and routes customer support inquiries into a single ticketing dashboard.</h3>

<h3>For an in depth rundown on Microsoft Azure visit this helpful guide <a href="https://github.com/mchajdecki/Microsoft-Azure">Microsoft Azure Full Tutorial</a>

<h2>This tutorial outlines the following</h2>
<ul>

<li><a href="#roles">Configure Roles</a></li>
<li><a href="#departments">Configure Departments</a></li>
<li><a href="#teams">Configure Teams</a></li>
<li><a href="#agents">Configure Agents(workers)</a></li>
<li><a href="#users">Configure Users(customers)</a></li>
<li><a href="#sla">Configure SLA</a></li>
<li><a href="#help">Configure Help Topics</a></li>
</ul>
</br>


<h1 id="roles"><i>Configure Roles</i></h1>
<h2>In osTicket, configuring roles means defining specific permission levels—such as the ability to delete tickets, edit threads, or assign tasks—that can be assigned to agents independent of their departmental access.</h2>

<p>
  <ol type="1">
     <li>Navigate to and Log into the Admin/Analyst section of osTicket to begin <a href="http://localhost/osTicket/scp/login.php">Admin/Analyst Login Page:</a></li></li>
    <li>Use the credentials set up in the pre-installation and configuration of osTicket.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/89b59c28a6e41f1756f5561e9cbf824138831781/images/Slide-1.jpg" alt="Slide_1"/>
</p>
<br>
<hr>


<p>
  <ol type="1">
    <li>Once logged in click on the Admin Panel button to continue.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/5741d134309dd1b8092fb9324a885f84510b4276/images/Slide-2.jpg" alt="Slide_2"/>
</p>
<br>
<hr>


<p>
  <ol type="1">
    <li>Click on agents.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/f11b60748b1fb8576c62b4ac5c4c3e2fb8c5c622/images/Slide-3.jpg" alt="Slide_3"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Click on roles.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/01edbadb71f475d8d952a83cf972aa6fa9d1c26e/images/Slide-4.jpg" alt="Slide_4"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>In the roles section we see all various types of access levels.</li>
    <li>Click on expanded access to continue.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/215175f95a4f776c747b86d4592949170f2d0113/images/Slide-5.jpg" alt="Slide_5"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Click on permissions.</li>
    <li>These are the checked permissions in the expanded access in roles.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/04df85904f0bc1ee79b0e0b153d764734a420b2c/images/Slide-6.jpg" alt="Slide_6"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Go back to --> Agents --> Roles and Click on Add New Role.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/7f55a4f11082399727c905c37c9f86d971898439/images/Slide-7.jpg" alt="Slide_7"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Name the new role i.e. Supreme Administrator.</li>
    <li>Click on Add Role.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/91bf1d1c18c092002aac4064bc486c1ae0774b71/images/Slide-8.jpg" alt="Slide_8"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Check all Permissions for the newly added role in the Tickets portion.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/09e48350b7ef548ebbab5130a3ad46c5a0a142b4/images/Slide-9.jpg" alt="Slide_9"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Check all Permissions for the newly added role in the Tasks portion.</li>
    <li>Click on Add Role to finish.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/8505f17122c2c5e9e200ab4c38054345086e60ff/images/Slide_10.jpg" alt="Slide_10"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Confirmation message displays that a new role has been added.</li>
    <li>New Supreme Administrator role displays.</li>
    <li>This concludes adding new role.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/4e41c0cbd204adf3d4be09c5d29b379f9791629d/images/Slide_11.jpg" alt="Slide_10"/>
</p>
<br>
<br>
<hr>



<h1 id="departments"><i>Configure Departments</i></h1>
<h2></h2>

<p>
  <ol type="1">
     <li></li>
  </ol>
</p>
<p>
<img src="" alt=""/>
</p>
<br>
<hr>


