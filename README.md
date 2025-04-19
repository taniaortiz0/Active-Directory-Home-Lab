# Active Directory Group Policy Management with PowerShell Automation

● Configured Windows Server 2022 as my Domain Controller (DC) and attached Windows 11 VM to domain.
● Created domain users, organizational units, and groups using Active Directory (AD) and assigned folders/permissions.
● Implementation and Management of Group Policy Objects along with maintenance on Windows DNS and DHCP services.
● Automated tasks using PowerShell for the creation of AD users with its parameters and resetting AD passwords.

![Windows Server 2022](https://github.com/user-attachments/assets/686d0760-915e-4029-ac08-00b2123c08e6)

Configured Windows Server 2022 as my Domain Controller (DC) and this will be utilized as the Default Gateway for the two NICs. 

![2 NICs](https://github.com/user-attachments/assets/a35df314-692a-4bb9-a6d1-5613e4cd8209)

Included two Network Adapters, one is to attach to NAT (Internet) and other one is to the Internal Network (Isolated). 
I then configured the Internal Network to set up the IP address, subnet mask, and DNS.

![AD DS](https://github.com/user-attachments/assets/383fb88e-41bb-492d-9bc7-858e74cab26b)

Next, I Installed AD DS (Active Directory Domain Services) and created a domain.

![image](https://github.com/user-attachments/assets/a789aaa0-0983-4311-ad63-602c99ba09fe)

I went to the Local Server to see my Domain being listed on the Properties section. 



I went ahead and got into the Windows Administrative Tools then into Active Directory Users and Computers to create Organizational Units (OUs). This includes a domain admin account, 

![image](https://github.com/user-attachments/assets/cb757ab0-767e-47af-8b93-c62316c455ef)

Next, I installed and configured RAS (Remote Access Server) with NAT (Network Address Translation). The Windows 11 client will be in a private-virtual network, but still be able to access the Internet through the DC. 
