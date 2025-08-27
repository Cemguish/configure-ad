
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Azure 
- PHP Manager for IIS
- Rewrite Module
- VC relist
- MySQL
- HeidiSQL
- osTicket

<h2>Configuration Steps</h2>

<p>
Log into azure make sure you enable virtual machines from the previous session.
  All credentials should be the same.
<img width="1704" height="926" alt="PIO 1" src="https://github.com/user-attachments/assets/4d254cf5-da36-4683-94e6-67e682499284" />
</p>

<p>
  Log into remote desktop 
<img width="1473" height="875" alt="PIO 2" src="https://github.com/user-attachments/assets/ea3c9df1-b504-4a3a-bbd4-12c3f6c1c0cb" />
</p>
<br />

<p>
    Next, copy and paste this URL into the search bar http://localhost/osTicket/scp/login.php 
  I will be using this for Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
<img width="1458" height="893" alt="PIO 3" src="https://github.com/user-attachments/assets/cded2f53-2231-43cb-bb3b-a248dd300c0d" />

</p><br />
<p>
   Open another window and copy and paste this URL into the search bar http://localhost/osTicket 
  I will be using this for End Users osTicket URL: http://localhost/osTicket 
  <img width="1678" height="737" alt="PIO 4" src="https://github.com/user-attachments/assets/2ed5b828-765a-4bce-a701-fd101aa421f9" />

</p>
<br />

<p>
  After login to osTicket I will be creating and few roles Supreme Admin, SysAdmins, Online Banking, Agent(Workers) and Users (Customers)
  Navigate to the double click > Agent panel 
<img width="1709" height="862" alt="PIO 5" src="https://github.com/user-attachments/assets/2b9f9cdc-d4d6-4206-87a5-e0d1d0642d7c" />
</p>


<p>
Next go to agent > Roles > Add new role. 
I will create a role called Supreme Admin.
Fill in the name box Supreme Admin.

<img width="1257" height="577" alt="PIO 7" src="https://github.com/user-attachments/assets/e7053edb-c19c-4deb-9061-3b6def896db6" />


</p>
<br />


<p>
  Then click on the Permissions tab and check all boxes.
  Click on the Task Tab and check all boxes.
  Click on knowledge base check the Premade box then add role
<img width="1103" height="757" alt="PIO 8" src="https://github.com/user-attachments/assets/4fb310e0-5a74-4665-afdc-2b02df7772fd" />

</p>

<p>
  After creating the role successfully you will see successfully added role to the top of the page in a green box.
<img width="1022" height="554" alt="PIO 10" src="https://github.com/user-attachments/assets/faa41a6d-6d29-4427-a0f9-ca62e323fb41" />

</p>
<br />

<p>
  Next, I will be creating a role for Departments. 
  Go back to the Admin panel > Agents > Departments add New "Department".
<img width="1168" height="495" alt="PIO 11" src="https://github.com/user-attachments/assets/e1f9ba60-22c4-4c44-957d-0f190bcfad27" />
</p>

<p>
  At the add department section for the parent leave it as Top level department > Name SysAdmins and create.
<img width="1033" height="981" alt="PIO 12" src="https://github.com/user-attachments/assets/5b935438-af86-47a6-8c43-ff9e07349664" />

</p>
<br /><p>
   After creating the SysAdmin Department successfully you will see successfully added role to the top of the page in a green box.
<img width="1100" height="532" alt="PIO 13" src="https://github.com/user-attachments/assets/7546be30-a1e1-465d-924d-b8c578468b74" />

</p>

<p>
Now I will create teams for Online banking
Go back to admin panel > Teams
Add New Teams name the team "Online Banking" 
Now Create Team
  <img width="1056" height="465" alt="PIO 14" src="https://github.com/user-attachments/assets/a23908e9-579c-410f-99da-2e296d5cabe0" />
</p>
<br />

<p>
After creating the Online Banking Team successfully you will see successfully added to the top of the page in a green box.
<img width="1027" height="805" alt="PIO 15" src="https://github.com/user-attachments/assets/38daeceb-203e-4f88-a564-8e136b1b485a" />
</p>



<p>
Now I will allow anyone (user/admins) to create tickets. This will allow end user to create tickets without an account.
Go to Admin Panel > Setting > User 
Make sure Registration Required box is unchecked.
Now go back to the admin panel.
<img width="1047" height="762" alt="PIO 16" src="https://github.com/user-attachments/assets/dae0461e-7196-4d82-a7a2-31e6f4bf5fdc" />
</p>
<br />


<p>
Now I will set up two Agent Accounts. Jane (Dept: SysAdmins) and John (Dept: Support)
Admin Panel > Agents > Add new Agents.
Fill in the relevant fields like  Name, email address, User name, and Set password.
Next, go to the access tab for the choose department and role. Add Department Support/SysAdmins add role Supreme Admin.
Click on the Teams Tab Add to "Online Banking" and Create
<img width="1028" height="973" alt="PIO 19" src="https://github.com/user-attachments/assets/937b0b48-427a-4b92-8a56-4f44831bbe18" />
</p>


<p>
Go back to the admin panel
Admin Panel > Agents > Add new Agents.
Fill in the relevant fields like  Name, email address, User name, and Set password.
Next, go to the access tab for the choose department and role. Add Department Support add role View Only click create.
Click Create
<img width="1084" height="626" alt="PIO 21" src="https://github.com/user-attachments/assets/b1522061-d7d9-4e1d-af3b-e4c24d934c4f" />
</p><br />

<p>
I will now setting up an account for 1 users.
Go back to the Agent panel > Go to Admin panel > user > add user
<img width="990" height="830" alt="PIO 22" src="https://github.com/user-attachments/assets/c7124f0d-4d7f-451f-8588-153870eb8c9c" />
</p><br />

<p>
In the user section fill in the relevant fields Email address and full name then Add user.
<img width="752" height="847" alt="PIO 23" src="https://github.com/user-attachments/assets/a16248e9-159e-41cb-b084-2172e83d74ac" />
</p><br />

<p>
  Now I will be creating 3 SLA's
Admin Panel > Manage > SLA.
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)
  <img width="997" height="919" alt="PIO 24" src="https://github.com/user-attachments/assets/acc77891-53c3-4dfc-9575-c2fb99645bb8" />
</p>
<br />


<p>
Admin Panel > Manage > SLA.
Add new SLA Plan complete the necessary fields Name, Grace period, and schedule. Now click on add plan.
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
<img width="1025" height="957" alt="image" src="https://github.com/user-attachments/assets/e0dfc424-e81a-4f09-b11a-5b401b50be6f" />
</p><br />
<p>

  <p>
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
<img width="1026" height="786" alt="PIO 26" src="https://github.com/user-attachments/assets/afd34fe6-7434-49a0-b7fd-dbb37c4c84f4" />
</p>

<p>
  Sev-C (Grace Period: 8 hours, Business Hours)
<img width="1034" height="926" alt="PIO 27" src="https://github.com/user-attachments/assets/a77e227d-b297-46cf-9654-2ad557f3fdcc" />
</p>

<p>
Go back to Admin panel
<img width="1012" height="922" alt="PIO 28" src="https://github.com/user-attachments/assets/a4cebfcd-cc32-4f59-b232-57b4e17a552e" />
</p><br />

<p>
Now, I will set up the Help topic/categories.
Admin Panel > Manage > Help Topics.
I will be setting up a few topics 
  
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other
<img width="1033" height="959" alt="PIO 29" src="https://github.com/user-attachments/assets/03f43208-8d23-42ae-ad52-06fa3ccb6275" />
</p><br />

<p>
Click add help topics 
Fill out the necessary fields
Topic: Business Critical Outage
Parent topic: Report Problem 
Add Topic
Go back to help topic > Add new Help Topic
<img width="1002" height="965" alt="PIO 30" src="https://github.com/user-attachments/assets/c2507334-85df-4cf0-9ed8-f5191a3355d5" />
</p><br />

<p>
  Click add help topics 
Fill in the necessary fields
Topic: Personal Computer Issues
Parent topic: Report Problem 
Add Topic
Go back to help topic > Add new Help Topic
<img width="1023" height="768" alt="PIO 31" src="https://github.com/user-attachments/assets/23a7b358-9531-435b-a6d3-79dcf313e27f" />
</p><br />


<p>
  Click add help topics 
Fill in the necessary fields
Topic: Equipment Request
Parent topic: Report Problem 
Add Topic
Go back to help topic > Add new Help Topic
<img width="1042" height="993" alt="PIO 32" src="https://github.com/user-attachments/assets/1a665eda-e036-4c41-8194-fe0df3ebd6ac" />

</p><br />

<p>
  Click add help topics 
Fill in the necessary fields
Topic: Password Reset
Parent topic: Report Problem 
Add Topic
Go back to help topic > Add new Help Topic
<img width="1054" height="929" alt="PIO 33" src="https://github.com/user-attachments/assets/79969f3c-1db9-48e5-9c58-3d4ea2e91b05" />
</p><br />


<p>
  Click add help topics 
Fill in the necessary fields
Topic: Other
Parent topic: Report Problem 
Add Topic
Go back to help topic > Add new Help Topic
<img width="1031" height="962" alt="PIO 34" src="https://github.com/user-attachments/assets/57ad936e-06e5-46b9-9a0d-287e1a2dd140" />
</p><br />

<p>
  Now osTicket is now set up and completed.
<img width="1049" height="955" alt="PIO 35" src="https://github.com/user-attachments/assets/5927f5d0-110f-43b2-947d-9aa2bba6758b" />

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>

