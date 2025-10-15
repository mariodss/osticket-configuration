<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users 
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<b>1) </b>Log in to your virtual machine and access osTicket via your web browser using the following links:
</p>
<p>
Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php 
</p>
<p>
End Users osTicket URL:
http://localhost/osTicket 
</p>
<br />

<p>
<img width="644" height="329" alt="image" src="https://github.com/user-attachments/assets/c196251f-4571-4ef7-b732-83a5f42ca0ac" />
<img width="647" height="254" alt="image" src="https://github.com/user-attachments/assets/6b5d0cdb-d4e7-456d-822c-6d51fadbc051" />

</p>
<p><b>2) </b>Configure Roles (for grouping permissions)</p>
<p>Admin Panel -> Agents -> Roles</p>
<p>-Supreme Admin</p>
<br />


<p>
<img width="650" height="536" alt="image" src="https://github.com/user-attachments/assets/f97779e6-1dc5-4de2-83d5-bf9c10cd5c8d" />
</p>
<p><b>3) </b>Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)</p>
<p>Admin Panel -> Agents -> Departments</p>
<p>-SysAdmins</p>
<br />

<p>
<img width="652" height="396" alt="image" src="https://github.com/user-attachments/assets/5baeb0b1-d0fc-462a-a17e-01e66073f119" />
</p>
<p><b>4) </b>Configure Teams</p>
<p>Admin Panel -> Agents -> Teams (Pull Agents from different Departments)</p>
<p>-Online Banking</p>
<br />

<p>
<img width="644" height="408" alt="image" src="https://github.com/user-attachments/assets/6c3c6e00-1476-4f1e-a97d-607b325cc625" />
</p>
<p><b>5) </b>Allow anyone to create tickets</p>
<p>Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)</p>
<p>-Registration Required: Require registration and login to create tickets </p>
<br />

<p>
<img width="640" height="489" alt="image" src="https://github.com/user-attachments/assets/bfa6bf78-c910-44a7-8f51-2bdc7c6349b4" />
<img width="641" height="312" alt="image" src="https://github.com/user-attachments/assets/27f84e07-d9a1-42f6-9d53-9833ce2736f0" />
<img width="638" height="241" alt="image" src="https://github.com/user-attachments/assets/4d0ce314-d9c7-4ab8-8d9b-294b00b88359" />

</p>
<p><b>6) </b>Configure Agents (workers)</p>
<p>Admin Panel -> Agents -> Add New</p>
<p>-Jane (Dept: SysAdmins) </p>
<p>-John (Dept: Support) </p>
<br />


<p>
<img width="642" height="458" alt="image" src="https://github.com/user-attachments/assets/37ce5e97-fcce-4332-9975-d9aa963875d5" />
</p>
<p><b>7) </b>Configure Users (customers)</p>
<p>Agent Panel -> Users -> Add New</p>
<p>-Karen </p>
<p>-Ken </p>
<br />

<p>
<img width="639" height="393" alt="image" src="https://github.com/user-attachments/assets/f1977cbd-86b2-4773-9abd-ce44c5b629f3" />
<img width="641" height="388" alt="image" src="https://github.com/user-attachments/assets/9469c1b5-1fa8-4efd-b62e-fd94affdca86" />
<img width="647" height="384" alt="image" src="https://github.com/user-attachments/assets/907fa5f3-eda9-4180-82c4-d1d158d768d6" />
</p>
<p><b>8) </b>Configure SLA</p>
<p>Admin Panel -> Manage -> SLA</p>
<p>-Sev-A (Grace Period: 1 hour, Schedule: 24/7)</p>
<p>-Sev-B (Grace Period: 4 hours, Schedule: 24/7)</p>
<p>-Sev-C (Grace Period: 8 hours, Business Hours)</p>
<br />

<p>
<img width="643" height="371" alt="image" src="https://github.com/user-attachments/assets/922eb5bd-2bbb-498c-bca7-bfe437caf4c4" />
<img width="646" height="375" alt="image" src="https://github.com/user-attachments/assets/b70f3d64-a18e-4198-9dfd-f11da8b9bf00" />
<img width="652" height="374" alt="image" src="https://github.com/user-attachments/assets/c31816b6-3d1b-41ef-b3a2-52e63d72fa44" />
<img width="643" height="369" alt="image" src="https://github.com/user-attachments/assets/c397adaa-0617-483b-8ab9-234e44f3cd6a" />
<img width="640" height="374" alt="image" src="https://github.com/user-attachments/assets/b119607e-890e-48d4-9474-6af7a1de61ac" />
</p>
<p><b>9) </b>Configure Help Topics (For when users create a ticket)</p>
<p>Admin Panel -> Manage -> Help Topics</p>
<p>-Business Critical Outage</p>
<p>-Personal Computer Issues</p>
<p>-Equipment Request</p>
<p>-Password Reset</p>
<p>-Other</p>
<br />
