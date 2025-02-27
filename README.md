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

- Understand the Interface
- Identify and distinguish between Agent Panel and Admin Panel
- Learn to navigate between the different panels and their respective functionalities
- Recognize how each panel serves different roles in the ticketing system

---

<h2>Configuration Steps</h2>

# osTicket Configuration Guide  

## 1. Setting Up [Roles](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)  

- Navigate to **Admin Panel → Agents → Roles**  
- Create a **Supreme Admin** role with full system permissions  
- Define role permissions for ticket management, task assignment, and system configuration  

## 2. Configuring [Departments](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)  

- Navigate to **Admin Panel → Agents → Departments**  
- Create department: **SysAdmins**  
- Configure department settings, including ticket visibility and access permissions  

## 3. Establishing [Teams](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html)

- Navigate to **Admin Panel → Agents → Teams**  
- Create team: **Online Banking**  
- Populate team with agents from different departments  
- Configure team permissions and responsibilities  

## 4. Managing User Access Settings  

- Navigate to **Admin Panel → Settings → User Settings**  
- Configure registration requirements for ticket creation  
- Set **Registration Required** option:  
  - ✅ "Require registration and login to create tickets"  

## 5. Setting Up [Agents (workers)](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)  

- Navigate to **Admin Panel → Agents → Add New**  
- Create agent accounts with appropriate credentials:  
  - **Jane** (Department: **SysAdmins**)  
  - **John** (Department: **Support**)  
- Assign appropriate roles and permissions to each agent  
- Configure agent access to tickets and departments  

## 6. Creating End [Users (customers)](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html)  

- Navigate to **Agent Panel → Users → Add New**  
- Create user accounts for:  
  - **Karen**  
  - **Ken**  
- Configure user information and access settings  
- Understand the difference between agents and end users  

## 7. Implementing Service Level Agreements [(SLAs)](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)  

- Navigate to **Admin Panel → Manage → SLA**  
- Create three distinct SLA plans:  
  - **Sev-A** (Grace Period: **1 hour**, Schedule: **24/7**)  
  - **Sev-B** (Grace Period: **4 hours**, Schedule: **24/7**)  
  - **Sev-C** (Grace Period: **8 hours**, **Business Hours**)  
- Understand how SLAs affect ticket resolution priorities and timelines

## 8. Configure [Help Topics](https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html) (For when users create a ticket)  

- Admin Panel -> Manage -> Help Topics
  - Business Critical Outage
  - Personal Computer Issues
  - Equipment Request
  - Password Reset
  - Other
