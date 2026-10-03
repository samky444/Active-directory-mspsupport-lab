\# Troubleshooting



\## Client Network Connectivity Issue



During the lab, Client 1 initially lost network connectivity and received an APIPA address in the `169.254.x.x` range.



\### Investigation



The issue was investigated systematically by checking:



\- VirtualBox network adapter configuration

\- Cable connection status

\- IP address configuration

\- Default gateway

\- DNS server configuration

\- Connectivity to the domain controller



The VirtualBox NAT Network was configured with DHCP disabled, so the client required a valid IP configuration.



\### Resolution



The virtual network adapter's \*\*Cable Connected\*\* setting was enabled and Client 1 was configured with:



\- IP Address: `10.0.2.21`

\- Subnet Mask: `255.255.255.0`

\- Gateway: `10.0.2.1`

\- DNS Server: `10.0.2.20`



\### Validation



Connectivity was verified using:



\- `ping 10.0.2.20`

\- `ping 10.0.2.1`

\- `ping 8.8.8.8`

\- `nslookup samlab.local`

\- `nslookup www.google.com`



The client successfully re-established connectivity with the domain controller and internet.



\## Troubleshooting Approach



The issue reinforced a structured IT troubleshooting process:



\*\*Physical/virtual connection → IP configuration → Gateway → DNS → Domain services → Group Policy\*\*

