# Active Directory Home Lab (In-Progress)

# Editing this ● Configured Windows Server 2022 as my Domain Controller (DC) and attached Windows 11 VM to domain.
● Created domain users, organizational units, and groups using Active Directory (AD) and assigned folders/permissions.
● Implementation and Management of Group Policy Objects along with maintenance on Windows DNS and DHCP services.
● Automated tasks using PowerShell for the creation of AD users with its parameters and resetting AD passwords. #

![Windows Server 2022](https://github.com/user-attachments/assets/686d0760-915e-4029-ac08-00b2123c08e6)

Configured Windows Server 2022 as my Domain Controller (DC) and this will be utilized as the Default Gateway for the two NICs. 

![2 NICs](https://github.com/user-attachments/assets/a35df314-692a-4bb9-a6d1-5613e4cd8209)

Included two Network Adapters, one is to attach to NAT (Internet) and other one is to the Internal Network (Isolated). 
I then configured the Internal Network to set up the IP address, subnet mask, and DNS.

![AD DS](https://github.com/user-attachments/assets/383fb88e-41bb-492d-9bc7-858e74cab26b)

Next, I Installed AD DS (Active Directory Domain Services) and created a domain.

![image](https://github.com/user-attachments/assets/a789aaa0-0983-4311-ad63-602c99ba09fe)

I went to the Local Server to see my Domain being listed on the Properties section. 

![domain admin](https://github.com/user-attachments/assets/6a71c432-4ba4-45d4-9e9f-0faabf9398b8)

I went ahead and got into the Windows Administrative Tools then into Active Directory Users and Computers to create a domain admin account. 

![image](https://github.com/user-attachments/assets/cb757ab0-767e-47af-8b93-c62316c455ef)

Next, I installed and configured RAS (Remote Access Server) with NAT (Network Address Translation). This will be utilized for the Windows 11 client to be in a private-virtual network, but still be able to access the Internet through the DC. 

![DHCP](https://github.com/user-attachments/assets/fdbd4e46-b9fc-4c6c-876e-7ec53647f126)

Next, I installed DHCP Server for the Windows 11 client to get an IP address which will give it access to the Internet meanwhile, it's in a private-internal network.

![powershell ise 2](https://github.com/user-attachments/assets/ae80e8bd-e1d7-4423-87c7-be2459d8ca98)

I utilize the command Set-ExecutionPolicy Unrestricted to be able to run PowerShell scripts that are download from the Internet. I then switched directories and executed the PowerShell script from this forked repository. [AD_PS](https://github.com/taniaortiz0/AD_PS)

![POWERSHELL Script generated +1000 users](https://github.com/user-attachments/assets/5874c100-28a7-4914-ae5f-8e8a483e3cea)

As we see, the custom PowerShell script created (1000+) users for the AD Lab.

![wINDOWS 11 BYPASS](https://github.com/user-attachments/assets/9b033512-7ae2-4385-b736-94c734cf3556)

I then configured Windows 11 for it to act as an Internal NIC and being able to obtain its IP address from the DHCP Server that I configured.


