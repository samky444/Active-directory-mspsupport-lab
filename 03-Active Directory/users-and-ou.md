\# Active Directory Users and OU Management



\## Overview



Active Directory was configured to provide centralized management of users within the `samlab.local` domain.



\## Users Created



The following domain user accounts were created:



\- Mary Johnson — `mary`

\- John Smith — `john`

\- Alex Brown — `alex`



\## Organizational Unit



An organizational unit named \*\*Lab Users\*\* was created within the `samlab.local` domain.



The three user accounts were moved into the \*\*Lab Users\*\* OU to provide centralized administration and allow user-based Group Policy to be applied.



\## Group Policy



The \*\*Folder Redirection - Lab Users\*\* Group Policy Object was linked to the \*\*Lab Users\*\* OU.



This configuration allows user-specific policies to be applied to accounts located within the OU.



\## Validation



Active Directory Users and Computers was used to verify the user accounts and their placement within the \*\*Lab Users\*\* OU.



\## Evidence



The screenshot in this folder shows the configured \*\*Lab Users\*\* OU and the domain user accounts.

