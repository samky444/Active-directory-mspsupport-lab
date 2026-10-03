\# Testing Results



\## Overview



The completed Active Directory environment was tested from the Windows 11 domain clients to verify connectivity, DNS, domain controller discovery, Group Policy, Folder Redirection, and NTFS security.



\## Test Results



| Test | Result |

|---|---|

| Group Policy processing | Successful |

| Client-to-server connectivity | Successful |

| `samlab.local` DNS resolution | Successful |

| Domain controller discovery | Successful |

| Mary's redirected folder access | Successful |

| Unauthorized access to Mary's folder | Denied as expected |

| Client 2 DNS resolution | Successful |



\## Commands Used



The following commands were used during validation:



\- `gpresult /r`

\- `ping 10.0.2.20`

\- `nslookup samlab.local`

\- `nltest /dsgetdc:samlab.local`



\## Security Validation



NTFS permissions were tested to confirm that a different domain user could not access Mary's protected redirected folder.



The access-denied result demonstrated that user data was appropriately restricted.



\## Conclusion



The tests confirmed that the Windows Server 2025 Active Directory environment was functioning across both Windows 11 clients, including domain services, DNS, Group Policy, Folder Redirection, and user data access controls.

