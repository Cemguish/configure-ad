
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

- Azure 
- PHP Manager for IIS
- Rewrite Module
- VC relist
- MySQL
- HeidiSQL
- osTicket

<h2>Configuration Steps</h2>

<p>
<b>Log into azure make sure you enable virtual machines from the previous session.</b>
  <li>All credentials should be the same.</li>
    <li>Log into remote desktop.</li><br> 
<img width="1704" height="926" alt="PIO 1" src="https://github.com/user-attachments/assets/4d254cf5-da36-4683-94e6-67e682499284" />
<img width="1473" height="875" alt="PIO 2" src="https://github.com/user-attachments/assets/ea3c9df1-b504-4a3a-bbd4-12c3f6c1c0cb" />
</p>
<br>

<p>
  <b>Next, copy and paste this URL into the search bar http://localhost/osTicket/scp/login.php</b> 
  <li>I will be using this for Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php</li>
  <li>Open another window and copy and paste this URL into the search bar http://localhost/osTicket</li> 
   <li>I will be using this for End Users osTicket URL: http://localhost/osTicket</li><br>  
<img width="1458" height="893" alt="PIO 3" src="https://github.com/user-attachments/assets/cded2f53-2231-43cb-bb3b-a248dd300c0d" /> 
<img width="1678" height="737" alt="PIO 4" src="https://github.com/user-attachments/assets/2ed5b828-765a-4bce-a701-fd101aa421f9" />
</p>
<br>

<p>
<b>After login to osTicket I will be creating and few roles.</b>
 <li>Roles such as Supreme Admin, SysAdmins, Online Banking, Agent(Workers) and Users (Customers)</li>
 <li>Navigate to the double click > Agent panel.</li>
 <li>Next go to agent > Roles > Add new role.</li> 
 <li>I will create a role called Supreme Admin.</li>
 <li>Fill in the name box Supreme Admin.</li>
 <li>Then click on the Permissions tab and check all boxes.</li>
 <li>Click on the Task Tab and check all boxes.</li>
 <li>Click on knowledge base check the Premade box then add role.</li>
 <li>After creating the role successfully you will see successfully added role to the top of the page in a green box.</li><br> 
<img width="1709" height="862" alt="PIO 5" src="https://github.com/user-attachments/assets/2b9f9cdc-d4d6-4206-87a5-e0d1d0642d7c" />
<img width="1257" height="577" alt="PIO 7" src="https://github.com/user-attachments/assets/e7053edb-c19c-4deb-9061-3b6def896db6" />
<img width="1103" height="757" alt="PIO 8" src="https://github.com/user-attachments/assets/4fb310e0-5a74-4665-afdc-2b02df7772fd" />
<img width="1022" height="554" alt="PIO 10" src="https://github.com/user-attachments/assets/faa41a6d-6d29-4427-a0f9-ca62e323fb41" />
</p>
<br>

<p>
  <b>Next, I will be creating a role for Departments.</b> 
   <li>Go back to the Admin panel > Agents > Departments add New "Department".</li>
   <li>At the add department section for the parent leave it as Top level department > Name SysAdmins and create.</li>
   <li>After creating the SysAdmin Department successfully you will see successfully added role to the top of the page in a green box.</li><br> 
<img width="1168" height="495" alt="PIO 11" src="https://github.com/user-attachments/assets/e1f9ba60-22c4-4c44-957d-0f190bcfad27" />
<img width="1033" height="981" alt="PIO 12" src="https://github.com/user-attachments/assets/5b935438-af86-47a6-8c43-ff9e07349664" />
<img width="1100" height="532" alt="PIO 13" src="https://github.com/user-attachments/assets/7546be30-a1e1-465d-924d-b8c578468b74" />
</p><br>

<p>
<b>Now I will create teams for Online banking.</b>
<li>Go back to admin panel > Teams.</li>
<li>Add New Teams name the team "Online Banking".</li> 
<li>Now Create Team.</li><br> 
<li>After creating the Online Banking Team successfully you will see successfully added to the top of the page in a green box.</li><br> 
<img width="1056" height="465" alt="PIO 14" src="https://github.com/user-attachments/assets/a23908e9-579c-410f-99da-2e296d5cabe0" />
<img width="1027" height="805" alt="PIO 15" src="https://github.com/user-attachments/assets/38daeceb-203e-4f88-a564-8e136b1b485a" />
</p>



<p>
<b>Now I will allow anyone (user/admins) to create tickets.</b> 
<li>This will allow end user to create tickets without an account.</li>
<li>Go to Admin Panel > Setting > User.</li> 
<li>Make sure Registration Required box is unchecked.</li>
<li>Now go back to the admin panel.</li><br> 
<img width="1047" height="762" alt="PIO 16" src="https://github.com/user-attachments/assets/dae0461e-7196-4d82-a7a2-31e6f4bf5fdc" />
</p>
<br>


<p>
<b>Now I will set up two Agent Accounts. Jane (Dept: SysAdmins) and John (Dept: Support)</b> 
<li>Admin Panel > Agents > Add new Agents.</li>
<li>Fill in the relevant fields like  Name, email address, User name, and Set password.</li>
<li>Next, go to the access tab for the choose department and role. Add Department Support/SysAdmins add role Supreme Admin.</li>
<li>Click on the Teams Tab Add to "Online Banking" and Create.</li><br> 
<img width="1028" height="973" alt="PIO 19" src="https://github.com/user-attachments/assets/937b0b48-427a-4b92-8a56-4f44831bbe18" />
</p>


<p>
<b>Go back to the admin panel.</b> 
<li>Admin Panel > Agents > Add new Agents.</li>
<li>Fill in the relevant fields like  Name, email address, User name, and Set password.</li>
<li>Next, go to the access tab for the choose department and role. Add Department Support add role View Only click create.</li>
<li>Click Create.</li><br> 
<img width="1084" height="626" alt="PIO 21" src="https://github.com/user-attachments/assets/b1522061-d7d9-4e1d-af3b-e4c24d934c4f" />
</p><br>

<p>
<b>I will now set up an account for 1 users.</b>
<li>Go back to the Agent panel > Go to Admin panel > user > add user.</li>
<li>In the user section fill in the relevant fields Email address and full name then Add user.</li><br> 
<img width="990" height="830" alt="PIO 22" src="https://github.com/user-attachments/assets/c7124f0d-4d7f-451f-8588-153870eb8c9c" />
<img width="752" height="847" alt="PIO 23" src="https://github.com/user-attachments/assets/a16248e9-159e-41cb-b084-2172e83d74ac" />
</p><br>

<p>
  <b>Now I will be creating 3 SLA's</b>
<dt>Admin Panel > Manage > SLA.</dt>
<dd>Sev-A (Grace Period: 1 hour, Schedule: 24/7)</dd>
<dd>Sev-B (Grace Period: 4 hours, Schedule: 24/7)</dd>
<dd>Sev-C (Grace Period: 8 hours, Business Hours)</dd><br>

<li>Admin Panel > Manage > SLA.</li>
<li>Add new SLA Plan complete the necessary fields Name, Grace period, and schedule. Now click on add plan.</li>
<li>Sev-A (Grace Period: 1 hour, Schedule: 24/7)</li>
<li>Add new SLA Plan complete the necessary fields Name, Grace period, and schedule. Now click on add plan.</li>
<li>Sev-B (Grace Period: 4 hours, Schedule: 24/7)</li>
<li>Add new SLA Plan complete the necessary fields Name, Grace period, and schedule. Now click on add plan.</li>
<li>Sev-C (Grace Period: 8 hours, Business Hours.</li>
<li>Go back to Admin panel.</li><br> 
<img width="997" height="919" alt="PIO 24" src="https://github.com/user-attachments/assets/acc77891-53c3-4dfc-9575-c2fb99645bb8" />
<img width="1025" height="957" alt="image" src="https://github.com/user-attachments/assets/e0dfc424-e81a-4f09-b11a-5b401b50be6f" />
<img width="1026" height="786" alt="PIO 26" src="https://github.com/user-attachments/assets/afd34fe6-7434-49a0-b7fd-dbb37c4c84f4" />
<img width="1034" height="926" alt="PIO 27" src="https://github.com/user-attachments/assets/a77e227d-b297-46cf-9654-2ad557f3fdcc" />
<img width="1012" height="922" alt="PIO 28" src="https://github.com/user-attachments/assets/a4cebfcd-cc32-4f59-b232-57b4e17a552e" />
</p><br>

<p>
<b>Now, I will set up the Help topic/categories.</b>
<li>Admin Panel > Manage > Help Topics.</li>
<li>I will be setting up a few topics.</li>
<li>Business Critical Outage</li>
<li>Personal Computer Issues</li>
<li>Equipment Request</li>
<li>Password Reset</li>
<li>Other</li><br>
<img width="1033" height="959" alt="PIO 29" src="https://github.com/user-attachments/assets/03f43208-8d23-42ae-ad52-06fa3ccb6275" /><br>


  <li>Click add help topics </li>
  <li>Fill out the necessary fields</li>
  <li>Topic: Business Critical Outage</li>
  <li>Parent topic: Report Problem</li> 
  <li>Add Topic</li>
  <li>Go back to help topic > Add new Help Topic</li><br>
<img width="1002" height="965" alt="PIO 30" src="https://github.com/user-attachments/assets/c2507334-85df-4cf0-9ed8-f5191a3355d5" /><br>


  <li>Click add help topics</li> 
  <li>Fill in the necessary fields</li>
  <li>Topic: Personal Computer Issues</li>
  <li>Parent topic: Report Problem</li> 
  <li>Add Topic</li>
  <li>Go back to help topic > Add new Help Topic</li><br>
<img width="1023" height="768" alt="PIO 31" src="https://github.com/user-attachments/assets/23a7b358-9531-435b-a6d3-79dcf313e27f" /><br>



  <li>Click add help topics</li> 
  <li>Fill in the necessary fields</li>
  <li>Topic: Equipment Request</li>
  <li>Parent topic: General Inquiry</li> 
  <li>Add Topic</li>
  <li>Go back to help topic > Add new Help Topic</li><br>
<img width="1042" height="993" alt="PIO 32" src="https://github.com/user-attachments/assets/1a665eda-e036-4c41-8194-fe0df3ebd6ac" /><br>


  <li>Click add help topics</li> 
  <li>Fill in the necessary fields</li>
  <li>Topic: Password Reset</li>
  <li>Parent topic: Report Problem</li> 
  <li>Add Topic</li>
  <li>Go back to help topic > Add new Help Topic</li><br>
<img width="1054" height="929" alt="PIO 33" src="https://github.com/user-attachments/assets/60386825-eea3-4195-b1a9-aa1848a0c1f4" /><br>


  <li>Click add help topics</li> 
  <li>Fill in the necessary fields</li>
  <li>Topic: Other</li>
  <li>Parent topic: Report Problem</li> 
  <li>Add Topic</li>
  <li>Go back to help topic > Add new Help Topic</li><br>
<img width="1031" height="962" alt="PIO 34" src="https://github.com/user-attachments/assets/57ad936e-06e5-46b9-9a0d-287e1a2dd140" /><br>
</p><br />

<p>
  <li>Now osTicket is now set up and completed ready to be used.</li><br>
<img width="1049" height="955" alt="PIO 35" src="https://github.com/user-attachments/assets/5927f5d0-110f-43b2-947d-9aa2bba6758b" />

</p>

