
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
  Now I will set up two Agent Accounts.
  Admin Panel > Agents > Add new Agents.
<img width="1057" height="498" alt="PIO 17" src="https://github.com/user-attachments/assets/f9716929-c422-4d72-98fe-a68b6edd1635" />
</p>


<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
