# Business-Network
This week I worked with a small team to build out and configure a small business network using GNS and FortiClient VPN.
Starting Topology
![image](https://github.com/LTGonzalez/Business-Network/assets/134319760/981e355c-022c-4e92-bba7-1dccc0c686c8)
Final network topology
![image](https://github.com/LTGonzalez/Business-Network/assets/134319760/46de35e3-78cc-416b-895d-24f2be7b5ae0)
With minimal guidance we set up a SMB (small/medium business) network, with a LAN, DMZ, and Guest network. We utilized a FortiNet firewall and configured both static and dynamic IP address for systems. We configured the interfaces in CLI and we configured the LAN interface and verified it was correct. We also created a Windows domain environment, an IIS server, a Windows FTP server, a Win10 workstation, a LAMP webserver running UNBUNTU, hosting a wiki, a Fortigate firewall, with a VIP for a DMZ webserver.
![image](https://github.com/LTGonzalez/Business-Network/assets/134319760/3a2def8e-80b0-4eb6-82d4-37e014e45e36)
![image](https://github.com/LTGonzalez/Business-Network/assets/134319760/751b2562-2f9e-4f1c-a898-43dc255833b6)
Setting up the DHCP
![image](https://github.com/LTGonzalez/Business-Network/assets/134319760/f57b292e-61f7-4abf-83b2-7172d44626ed)
Once the LAN and DHCP and DNS servers were set up we also added a WIN 2012 server to fill the Active Directory Domain Services role and installed Active Directory. Once the directory was created we added users and admin and group policies.
![image](https://github.com/LTGonzalez/Business-Network/assets/134319760/8802b762-8ad8-41b2-a0bd-16b920b9b75e)
Next we added a server for Internet Information Services "IIS" and created a LAMP (Linux, Apache, MySQL, PHP/Perl/Python) webserver on the DMZ network.
![image](https://github.com/LTGonzalez/Business-Network/assets/134319760/13be64bd-b1c8-4555-aec1-7b0e1743e998)
We configured a DokuWiki to document our work and process.
![image](https://github.com/LTGonzalez/Business-Network/assets/134319760/460c18da-c9bf-45f6-9d46-9ed028c344ef)
We then created an FTP server on the DMZ network. This allowsus to access files from the server from outside of the network. Below is also a screenshot showing access from an internet browser.
![image](https://github.com/LTGonzalez/Business-Network/assets/134319760/8da1b386-7480-4448-ac7a-cdac00acc18f)
At the end we ran a vulnerability scan using Greenbone and created our report.
![image](https://github.com/LTGonzalez/Business-Network/assets/134319760/9233fae9-f7c4-41f4-ac1f-c343b2f7aa0f)
