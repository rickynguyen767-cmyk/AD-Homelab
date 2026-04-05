# Active Directory Lab

## Overview
This project demonstrates a Windows Server Active Directory environment with domain services, user management, and group policies.

## Objectives
- Deploy AD DS
- Configure users and groups
- Implement Group Policy Objects (GPOs)
- Simulate an enterprise environment

## Environment
- Windows Server 2025
- Windows 11 client
- VirtualBox

## Architecture
<img src="images/Architecture/Active%20Directory.jpg" alt="Active Directory Architecture" width="400"/>

## Set Up
Configure virtual machines
- 1 server, 2 Hosts
<img src="images/Architecture/VirtualMachines.jpg" alt="Created Virtual Machines"/>

- Configure Private network for Machines
<img src="images/Architecture/CreateAnIsolatedNetwork.jpg" width="600"/>

- Add VMHosts to private network
<img src="images/Architecture/AddVMToNetwork.jpg" width="600"/>

- Set up Advanced Directory by clicking on "Add Roles and Features" in Server Manager
<img src="images/Architecture/SetUpAD.jpg" width="600"/>

- Go to the "Server Roles" tab and check "Active Directory Domain Services", then continue to install AD
<img src="images/Architecture/InstallAD.jpg" width="600"/>

- Afterwards, click on the flag icon on the top right of the screen and promote the server to a Domain Controller
<img src="images/Architecture/Promote.jpg" width="600"/>

- Create a new forest and create a "Root Domain Name" and Password, then continue and install settings
<img src="images/Architecture/CreateForest.jpg" width="600"/>

- After rebooting, go to Tools>Active Directory Users and Computers>(Domain name)>Users to create users
<img src="images/Architecture/CreateUser.jpg" width="600"/>

- Now that the server has been set up, go back to the host machines to finish adding them to the domain. Search "Access Work or School"
<img src="images/Architecture/AccessWork.jpg" width="600"/>

- Click "Join Local Active Directory"
<img src="images/Architecture/JoinAD.jpg" width="600"/>

- Enter Root Domain, User's sign-in information, and it's finished
<img src="images/Architecture/EnterUserInfo.jpg" width="600"/>
<img src="images/Architecture/UserFinished.jpg" width="600"/>
