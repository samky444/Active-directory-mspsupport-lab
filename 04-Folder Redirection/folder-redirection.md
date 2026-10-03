\# Folder Redirection



\## Overview



Folder Redirection was configured through Group Policy to redirect users' Documents folders to a network share hosted on the Windows Server 2025 domain controller.



\## Configuration



\- Group Policy Object: `Folder Redirection - Lab Users`

\- Organizational Unit: `Lab Users`

\- Redirected Folder: Documents

\- Network Share: `\\\\10.0.2.20\\UserData$`



The GPO was linked to the \*\*Lab Users\*\* OU so that the configuration would apply to the domain users in that OU.



\## Network Share



A hidden network share named `UserData$` was created on the domain controller.



The underlying folder was:



`C:\\UserData`



User folders were created within the share and secured with NTFS permissions.



\## Security



NTFS permissions were configured so that users could access their own redirected data while preventing unauthorized access to another user's folder.



For example, Mary could access her redirected folder, while John was denied access to Mary's protected folder.



\## Validation



Folder Redirection was tested by logging in as a domain user and accessing the redirected Documents location.



The configuration was also verified through Group Policy processing and direct access to the network share.



\## Evidence



The screenshots in this folder document the Folder Redirection GPO, redirected user folders, and the associated configuration.

