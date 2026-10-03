\# Domain Controller Setup



\## Overview



Windows Server 2025 was configured as the domain controller for a dedicated Active Directory lab environment.



\## Server Configuration



\- Operating System: Windows Server 2025 Standard Evaluation (Desktop Experience)

\- Active Directory Domain Services: Installed

\- DNS Server: Installed and configured

\- Domain: `samlab.local`

\- NetBIOS Name: `SAMLAB`

\- Domain Controller IP Address: `10.0.2.20`

\- Network: `NatNetwork`

\- Network Range: `10.0.2.0/24`



\## Active Directory Configuration



The server was promoted to a domain controller and configured with:



\- Active Directory Domain Services

\- DNS

\- Global Catalog

\- `samlab.local` Active Directory domain



\## Validation



The domain controller configuration was validated from the Windows 11 clients using:



\- `ping 10.0.2.20`

\- `nslookup samlab.local`

\- `nltest /dsgetdc:samlab.local`



These tests confirmed network connectivity, DNS resolution, and successful domain controller discovery.



\## Evidence



See the screenshots in this folder for visual evidence of the Windows Server 2025 domain controller configuration.

