\# Group Policy Logon Script



\## Overview



A Windows batch logon script was created and assigned through Group Policy to automatically place a Support Portal shortcut on the desktop of domain users.



\## Script



The script was named:



`SupportPortal.bat`



It was stored in the domain SYSVOL scripts directory:



`C:\\Windows\\SYSVOL\\sysvol\\samlab.local\\scripts`



\## Function



The script creates an Internet shortcut on the user's desktop that points to the Microsoft website.



The purpose of the exercise was to demonstrate how a Group Policy logon script can automate a standard desktop configuration for domain users.



\## Group Policy Configuration



The script was configured under:



\*\*User Configuration → Policies → Windows Settings → Scripts (Logon/Logoff) → Logon\*\*



The `SupportPortal.bat` script was assigned as a logon script.



\## Validation



The script was tested by logging in as the domain user Mary and John on a Windows 11 clients.



After Group Policy processing, the \*\*Support Portal\*\* shortcut appeared on the user's desktop.



\## Evidence



The screenshots in this folder show the logon script configuration and the resulting Support Portal shortcut on the Windows 11 client desktop.

