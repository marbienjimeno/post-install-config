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
- Allow anyone to create tickets
- Configure Agents
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

**Configure Roles**
<p>
  We'll begin by configuring additional roles in os Ticket. Go to the Admin Panel. Go to the Agents tab and select Roles. Click Add New Role. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/4cd005b7-441c-4f48-ab92-adcd8e0b1558)

<br />

<p>
  We'll name the new role "Supreme Admin". Go to Permissions and give this role all the available permissions. Click Add Role.
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/5bdb3441-4f92-4233-9aec-cb9940bb154e)

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/85ff22f6-209c-41bf-8ff3-d34f2e0be6b1)

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/d3d53ac3-461f-4823-bc87-b50f5042c9e7)

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/7b80be09-f2b0-402b-9c21-088a8bd2476e)

**Configure Departments**
<p>
  Now we will configure additional Departments. In the Agents tab, select Departments. Click Add New Department.
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/c5308a0c-e381-4eb7-aad6-43278a6f6bf1)

<p>
  We'll name the new department "System Administrators" and keep the other default settings. Click Create Dept.
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/2c6161f7-7eb2-44fc-985b-4cda3d41f8dd)

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/63dae9c8-6533-4751-9bdb-9dbc8c6ae3b2)

**Configure Teams**
<p>
  We will now configure the Teams in our osTicket system. In the Agents tab, go to Teams. Click Add New Team. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/7be8ebe3-f904-4c7f-b372-42881aa8c31a)

<p>
  For the name of the new team, enter Level II Support. Go to the Members tab and add yourself to the Level II Support team. Click Create Team. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/2d6cfc5b-fbb8-4fd1-b9f5-0acaa97a3688)

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/4ad159a1-700e-4b64-8573-dc816730b536)

**Allow anyone to create tickets**
<p>
  Now we will configure osTicket so that anyone can create tickets, whether they have an account or not. In the Admin Panel, go to the Settings tab. Select Users. Under Authentication Settings, make sure the Registration Required field is left unchecked. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/f02d65e3-09d6-4e5e-82ea-9d75fdcbad42)

**Configure Agents**
<p>
  Now we'll configure the Agents in our osTicket system. Agents are the helpdesk professionals that will respond to the tickets created. Go to the Agents tab and select Agents. Click Add New Agent.
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/b0968cb9-0b85-4554-8475-cf655c79d7fb)

<p>
  For the first new agent, we'll use the name "Jane Doe" and the email "jane.doe@osticket.com". For the username, we'll enter "jane.doe" and set the password to "Password1". Make sure to record the username and password for future reference. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/cbaac90c-240e-45b1-9ce1-4e3aaeed153e)

<p>
  Go to the Access tab. Under Primary Department, select System Administrators with a Supreme Admin role. Under Extended Access, add Support with a Supreme Admin role. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/6f817e96-df94-4777-a52c-0a38de474f1d)

<p>
  Go to the Teams tab and add Jane Doe to the Level II Support team. Click Create. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/7ada930e-dbfe-43d4-9fb9-4dbf55c99343)

<p>
  After successfully adding Jane doe as an agent, go back to Agents and click Add New Agent to add another agent. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/ba295408-25fe-4cc4-86da-1582534d96c2)

<p>
  For the second new agent, we'll give it the name "John Doe" and the email "john.doe@osticket.com". For username, we'll use "john.doe" and set the password as "Password1".
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/1d6a0a05-37a8-4e25-a26b-5d275be3cea9)

<p>
  Go to the Access tab. Under Primary Department, select Support with an All Access role. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/6c056e7b-9d90-459b-8d7c-9a5a38d86c56)

<p>
  Go to the Teams tab and add John Doe to the Level I Support team. Click Create. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/c7d2d76d-e2f8-4469-a0ce-70f3dffc5351)

**Configure Users**
<p>
  Now we will configure the Users of our osTicket system. Users will create the tickets that agents respond to. Go to the Agents Panel and select the Users tab. Click Add User. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/fdea325a-b203-4485-b7f0-481edb7fc7f4)

<p>
  For the first new user, we'll enter the email address "karen@osticket.com" and the full name "Karen Kove". Click Add User. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/f97aa861-2699-4afc-b13a-3d3c4b6604aa)

<p>
  We will add another user. For the email address, we'll use "ken@osticket.com". For the full name, we'll use "Ken Kount". Click Add User.
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/13cc5305-0f1d-473b-8f99-f1277964859a)

**Configure SLA**
<p>
  Now we will configure SLA's for our ostTicket system. SLA stands for "Service Level Agreement", and it provides a length of time in which tickets are expected to be closed. Go to the Admin panel and select the Manage tab. Select SLA. Click on Add New SLA Plan.
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/09384a2e-2947-4dce-851b-a43683e843d1)

<p>
  For the first new SLA, we'll name it SEV-A. For Grace Period, we'll put 1 hour. For Schedule, select 24/7. Click Add Plan. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/6a23e806-3cb3-4140-a5b0-f784cea3b48a)

<p>
  For the second new SLA, we'll name it SEV-B. For Grace Period, enter 4 hours. For Schedule, select 24/7. Click Add Plan. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/eb2e225f-7a58-4da6-9916-90b63ea0a85c)

<p>
  For the third new SLA, we'll name it SEV-C. For Grace Period, enter 8 hours. For Schedule, select Monday - Friday 8am - 5pm with U.S. Holidays. Click Add Plan. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/40088576-39cf-476a-9437-d638dbfe3dc9)

**Configure Help Topics**
<p>
  Lastly, we will configure the Help Topics avaliable in our osTicket system. Help Topics help to streamline the ticket creation process for users. In the Manage tab, select Help Topics. Click on Add New Help Topic. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/8b936ff6-8871-4ac1-9fd7-c2366b9a7d66)

<p>
  For the first new help topic, enter "Business Critical Outage". Click Add Topic. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/933c5fa5-2c26-4ea3-b347-818f76866cf8)

<p>
  For the second new help topic, enter "Personal Computer Issues". Click Add Topic. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/25cb375b-bca1-46cb-a473-c52d1269702b)

<p>
  For the third new help topic, enter "Equipment Request". Click Add Topic. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/61a2ab8a-5d9f-4289-a1e4-48f838c53625)

<p>
  For the last new help topic, enter "Password Reset". Click Add Topic. 
</p>

![image](https://github.com/marbienjimeno/post-install-config/assets/29347863/2237cbbe-e33a-43f8-9edc-30ed95e6c72a)

**Conclusion**
<p>
  We have successfully performed the post-installation configuration of our osTicket system. In the next section, we will follow the lifecycle of tickets, starting from the intake of the tickets to their resolution using the osTicket system.
</p>
