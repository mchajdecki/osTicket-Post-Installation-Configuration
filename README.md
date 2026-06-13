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
<li><a href="#allow">Configure Allowing Ticket Creators</a></li>
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
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/4e41c0cbd204adf3d4be09c5d29b379f9791629d/images/Slide_11.jpg" alt="Slide_11"/>
</p>
<br>
<br>
<hr>



<h1 id="departments"><i>Configure Departments</i></h1>
<h2>In osTicket, departments are organizational categories used to automatically route incoming support tickets to the appropriate team of agents based on the specific issue type or service tier.</h2>

<p>
  <ol type="1">
     <li>In the Admin panel - select Agents --> Departments</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/4bd7d8ad49fc8d297204ff20a1b4c006f5350362/images/Slide_12.jpg" alt="Slide_12"/>
</p>
<br>
<hr>


<p>
  <ol type="1">
    <li>Click on Add New Department.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/5b0b24f572716adc2210e9026aeb8761e53ebce9/images/Slide_13.jpg" alt="Slide_13"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Here is a breakdown of each section.</li>
    <ul>
<li>Department Information: Defines the department's core identity, visibility, SLA schedules, and ticket assignment rules.</li>
<li>Outgoing Email Settings: Determines the specific email address and template used for outgoing staff replies.</li>
<li>Autoresponder Settings: Toggles automatic confirmation emails for new tickets and user messages.</li>
<li>Alerts and Notices: Specifies which internal staff members receive notifications about ticket activity.</li>
<li>Department Signature: A standardized text block automatically appended to the bottom of staff replies.</li>
    </ul>
    <li>Fill in the information with the guide above for this example tutorial.</li>
    <li>Click on create dept to finish.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/edca6e5f3250bfe4bbb1e2067079e9fe1df9ef59/images/Slide_14.jpg" alt="Slide_14"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Successfull added new department messsage will display.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/2359eb8858626de477a140f2d90eed35f3cd7971/images/Slide_15.jpg" alt="Slide_15"/>
</p>
<br>
<br>
<hr>


<h1 id="teams"><i>Configure Teams</i></h1>
<h2>In osTicket, configuring teams creates cross-departmental groups of agents, enabling seamless collaboration and shared assignment on specialized tickets that require multiple areas of expertise.</h2>

<p>
  <ol type="1">
     <li>In the Admin Panel click on Teams.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/8dd13c6161e00454061f7f026d7074377b90c435/images/Slide_16.jpg" alt="Slide_16"/>
</p>
<br>
<hr>


<p>
  <ol type="1">
    <li>Click on Add New Team.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/8d8adebec4faccde27c08837499566f02799dd63/images/Slide_17.jpg" alt="Slide_17"/>
</p>
<br>
<hr>


<p>
  <ol type="1">
    <li>Click on Members.</li>
    <li>In this example we havent added any members yet, choose your own account for this tutorial.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/e11d8925ef859303a13b9cb5ac5bda24037b04f2/images/Slide_18.jpg" alt="Slide_18/>
</p>
<br>
<hr>


<p>
  <ol type="1">
    <li>Go back to Team.</li>
    <li>Name the team to a specific brand such as i.e. Online Banking.</li>
    <li>Leave the rest of the options and click on Create Team.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/c4745b08427175609fb1f593469ce30331b60294/images/Slide_19.jpg" alt="Slide_19"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Successfully added team message will display.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/12cc16ac90ce767113bae09051dbaac6039facd6/images/Slide_20.jpg" alt="Slide_20"/>
</p>
<br>
<br>
<hr>



<h1 id="allow"><i>Configure Allowing Ticket Creators.</i></h1>
<h2>Enabling a setting to allow users to quickly submit support tickets as guests without needing to register for an account or log in.</h2>

<p>
  <ol type="1">
     <li>Click on Settings --> Users.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/6814fda216db17e935ffb7293f5b1f0a6d6aa0b6/images/Slide_21.jpg" alt="Slide_21"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Make sure the Registration Required box is unchecked.</li>
    <li>Click on Save Changes to finish.</li>
    <li>Successfully updated User Settings and Options Message will display.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/be69988e3d162ca835ae800cf1ca3e55e9a3e169/images/Slide_22.jpg" alt="Slide_22"/>
</p>
<br>
<br>
<hr>



<h1 id="agents"><i>Configure Agents</i></h1>
<h2>In osTicket and this section we set up staff accounts, define their roles and permissions, and assign them to specific departments so your team can effectively manage and resolve incoming tickets</h2>

<p>
  <ol type="1">
     <li>Click on Agents to add new agent.s</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/f9f28662e74763a1ab0a444db354cfa4696f6265/images/Slide_23.jpg" alt="Slide_23"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Click Add New Agent.</li>
    <li>Create a "fake" name - email address and username for this tutorial.</li>
    <li>Select the department previously created i.e. Networking Issues with the Supreme Administrator Role.</li>
    <li>In Teams select the previously created Online Banking Team.</li>
    <li>Successfully Added a mew agent message displays.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/2b636d06efaf467f84f69bf1c80c5ca714adbf10/images/Slide_24.jpg" alt="Slide_24"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>Add another Agent i.e. Mark Smith.</li>
    <li>In access options choose only the Support and View only permissions.</li>
    <li>Click on Create to finish.</li>
    <li>Succesfully added new agent i.e Mark Smith message displays.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/6caf79f221bb9282745e5fcc6e13d451848ad428/images/Slide_25.jpg" alt="Slide_25"/>
</p>
<br>
<hr>

<p>
  <ol type="1">
    <li>To set up a password, nagivate to the agent and click on Set Password.</li>
    <li>Make sure the Send the agent a password reset email box is unchecked.</li>
    <li>Type in a new password and click update to set the log in password for a particular agent.</li>
  </ol>
</p>
<p>
<img src="https://github.com/mchajdecki/osTicket-Post-Installation-Configuration/blob/274044ffa897f2c0c67853f859796db62325f123/images/Slide_26.jpg" alt="Slide_26"/>
</p>
<br>
<hr>


<h1 id="allow"><i>Configure Users.</i></h1>
<h2></h2>

<p>
  <ol type="1">
     <li></li>
  </ol>
</p>
<p>
<img src="" alt="Slide_27"/>
</p>
<br>
<hr>

