<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-installation configuration of the open-source help desk ticketing system, osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Configuration Steps</h2>

<p>
  After successfully configuring osTicket, we will move on to system administration duties, beginning with setting up new support desk roles.  We will be able to efficiently manage user access and permissions as a result.
  <br />
  </p>
<p>
<img src="https://github.com/user-attachments/assets/680335fd-30c6-4767-ae7c-7b4fe47b1951"/>

  <img src="https://github.com/user-attachments/assets/10be3c3d-eca6-4fb1-8796-1766750b9913"/>

  <img src="https://github.com/user-attachments/assets/f196a0d3-df2f-44f6-96de-673a10281cbb"/>
</p>
<p>
Navigate to the Admin Panel -> Agents -> Roles to set up new roles in the help desk.  Select "Add new role" and type the new role's name, like "Supreme Admin."  This will enable us to specify the role's responsibilities and permissions.  All permissions will be granted to the Supreme Admin role since we are creating one.  To grant complete administrative access, we must make sure that every permission that is available is chosen for this role.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/353a001b-d0fa-4821-b01d-3fd4a2e0ecf1"/>

  <img src="https://github.com/user-attachments/assets/da5ec2c1-5cb7-4d39-83f7-91d0dda0e5a4"/>
</p>
<p>
We will then set up the departments.  On the Agents tab, click the "Departments" button.  A new department can be created here, and each agent will be assigned to a particular department according to their position within the help desk.  Establish a department called "SysAdmins" to act as the Supreme Admins' assigned department.  Within the Departments tab, you can adjust other settings like SLAs, managers, and email configurations to suit the operational requirements of your help desk.



</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/f959c33f-a83d-43b0-acd5-dce83d4feee3"/>
  <img src="https://github.com/user-attachments/assets/4a80145e-9d88-41eb-b285-47a67ca4526c"/>
</p>
<p>
Next, we'll discuss the teams.  Go to Admin Panel -> Agents -> Teams to set up teams.  Teams enable agents from various departments to work together efficiently. On this occasion, we will form a team for the online banking division. 


</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/2f55b864-6fde-49a9-8921-e34089f67785"/>
</p>
<p>
We must remove the registration requirement so that anyone can create tickets.  We need to go to Admin Panel -> Settings -> User Settings in order to accomplish this.  Unregistered users can submit tickets without requiring an account if the "Require registration and login to create tickets" option is unchecked.

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/4c0728d6-8273-4381-83ca-ee851179a4e7s"/>
  <img src="https://github.com/user-attachments/assets/90a0ff6b-adee-40c3-989f-7187ee122b7f"/>
  <img src="https://github.com/user-attachments/assets/805edc4a-c41d-4b69-94ed-08df7fddd963"/>
</p>
<p>
Agents will then be added to the system. Go to Admin Panel -> Agents -> Add New to set up agents (workers).  To set up the agent's profile and permissions, enter the required information, including their name, email address, department, and assigned role. This time, we'll include agent Jane Doe.  We will go to the access tab and designate "SysAdmins" as her primary department in order to give her permissions.


</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/51228b39-0be7-4df9-af97-bce1f1c1c5cb"/>
</p>
<p>
Go to Agent Panel -> Users -> Add New to configure users (customers).  To allow them to submit and manage their tickets, we will add the user Karen, who will enter her information, including her name and email address.

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/9d247e26-7f20-43cc-b652-c8b82d9fe070"/>
<img src="https://github.com/user-attachments/assets/56f3e64a-a4c5-4d14-abfe-35e84ebe2858"/>
  
</p>
<p>
We will then move on to help topics.  Go to Admin Panel -> Manage -> Help Topics to set up help topics for user ticket creation.  These subjects will help users properly classify their tickets.  We developed a "busineses critical outage" help topic for this example.


</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/3c3d8bb5-2c69-4a5c-bb0c-b1fd44fe028d"/>
<img src="https://github.com/user-attachments/assets/27088e68-08da-4853-8ed8-73fa5b7e3de2"/>
  
</p>
<p>
We will then move on to SLAs.  Go to Admin Panel -> Manage -> SLA  to add new SLA plans.  Tickets need to have SLA in order to determine its severity and amount of time needed for it to be finished. We added a "Sev-A" SLA  for this example.


</p>
<br />
Finally we have succsefully configered osTicket Roles,Departments, Teams, Agents, Users and Help topics
