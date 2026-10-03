\# Active Directory \& IT Support Lab



\## Project Overview



This project documents a hands-on Windows Server 2025 Active Directory and IT support lab built in VirtualBox.



The lab simulates a small business domain environment and demonstrates practical skills in Active Directory, DNS, Group Policy, Windows client administration, network troubleshooting, file permissions, and user support.



\## Environment



\- Windows Server 2025

\- Windows 11 Client 1

\- Windows 11 Client 2

\- VirtualBox

\- Active Directory Domain Services (AD DS)

\- DNS

\- Group Policy

\- Domain: `samlab.local`

\- Domain Controller IP: `10.0.2.20`

\- NAT Network: `10.0.2.0/24`



\## Skills Demonstrated



\- Active Directory domain administration

\- Domain user and OU management

\- Windows 11 domain joining

\- DNS configuration and troubleshooting

\- Group Policy management

\- Folder Redirection

\- NTFS permissions and access control

\- Logon scripts

\- Windows networking

\- Client-to-server troubleshooting

\- Domain controller discovery

\- IT support troubleshooting methodology



\## Project Components



\### 1. Domain Controller



Configured Windows Server 2025 as the Active Directory domain controller for `samlab.local`.



\### 2. Domain-Joined Clients



Joined two Windows 11 clients to the `samlab.local` domain.



\### 3. Active Directory



Created domain users and organized them within the `Lab Users` organizational unit.



\### 4. Folder Redirection



Configured user Documents folders to redirect to a secured network share on the domain controller.



\### 5. Login Script



Created a Group Policy logon script that deploys a Support Portal shortcut to the user's desktop.



\### 6. Troubleshooting



Documented network, DNS, Group Policy, and client connectivity troubleshooting performed during the project.



\### 7. Testing Results



Verified domain connectivity, DNS resolution, Group Policy application, Folder Redirection, NTFS security, and domain controller discovery.



\## Key Troubleshooting Example



During the project, a Windows 11 client experienced network connectivity problems and received an APIPA address.



I systematically checked the VirtualBox network configuration, cable connection, IP addressing, gateway, and DNS configuration. After correcting the network configuration and assigning the appropriate client IP and DNS settings, connectivity to the domain controller and internet was restored.



This reinforced a structured troubleshooting approach:



\*\*Network connectivity → IP configuration → DNS → Domain connectivity → Group Policy → Permissions\*\*



\## Project Outcome



The completed lab demonstrates a functional Windows domain environment with two Windows 11 clients, centralized user management, Group Policy, Folder Redirection, secured user data, and a working logon script.



This project was completed as a hands-on learning and portfolio project to demonstrate practical Windows and IT support skills.

