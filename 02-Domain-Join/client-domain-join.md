\# Windows 11 Domain Join



\## Overview



Two Windows 11 virtual machines were configured as domain-joined clients in the `samlab.local` Active Directory environment.



\## Client Configuration



\- Client 1: Windows 11

\- Client 2: Windows 11

\- Active Directory Domain: `samlab.local`

\- Domain Controller: Windows Server 2025

\- Domain Controller IP: `10.0.2.20`



\## Domain Join



Both Windows 11 clients were successfully joined to the `samlab.local` domain.



Domain membership was verified through the Windows system properties on each client.



\## Validation



Client connectivity and domain services were tested using:



\- `ping 10.0.2.20`

\- `nslookup samlab.local`

\- `nltest /dsgetdc:samlab.local`

\- `gpresult /r`



These tests verified communication with the domain controller, DNS name resolution, domain controller discovery, and Group Policy processing.



\## Evidence



The screenshots in this folder document the successful domain membership of both Windows 11 clients.

