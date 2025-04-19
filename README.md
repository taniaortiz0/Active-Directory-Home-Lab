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



Next, I Installed AD DS (Active Directory Domain Services) and created a domain. 
