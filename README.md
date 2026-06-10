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

- Admin/Analyst Login Page: <a href="http://localhost/osTicket/scp/login.php">Admin/Analyst Login where you configure settings on the back end for osTicket.</a>

- End Users osTicket URL: <a href="http://localhost/osTicket"> End Users osTicket URL, essentially a help desk worker that works on tickets.</a> 

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
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/618febc739ce97aadab23b15ca8160badbbaba46/images/Slide_1.jpg" alt="Slide_1"/>
</p>
<br>
<hr>


<p>
  <ol type="1">
    <li>Once logged in click on the Admin Panel button to continue.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/2716d336ea141034c080615d34c1d2a6bedda4c9/images/Slide_2.jpg" alt="Slide_2"/>
</p>
<br>
<hr>
