<h1>Home Data Center Lab</h1>


<h2>Description</h2>

<p>This project simulates a small enterprise-style data center environment using virtualized Linux and Windows systems. The lab focuses on core infrastructure services including DNS, IP configuration, and network troubleshooting within a controlled environment.

The objective was to gain hands-on experience with Linux-based system administration and internal DNS services, while reinforcing networking fundamentals used in real-world NOC and infrastructure roles.</p>


<b>Environment & Technologies</b>
<ul>
<li>Ubuntu Server (DNS+ system administration</li>
<li>BIND9 (DNS server)</li>
 <li>Netplan (network configuration)</li>
 <li>systemd (service configuration)</li>
</ul>

<b>Networking & Tools</b>
<ul>
<li>TCP/IP, Static Addressing</li>
<li>ip,ping,dig,resolvectl</li>
 <li>Virtualized networking</li>
</ul>

<b>Key Configurations</b>
<ul>
<li>Configured static IP addressing using Netplan</li>
<li>Deployed and configured BIND9 DNS server</li>
 <li>Created forward and reverse lookup zones</li>
 <li>Enabled internal name resolution between systems</li>
 <li>Managed DNS and system services using systemctl</li>
 <li>Configured client system to use internal DNS server</li>
</ul>

<b>Troubleshooting & Validation</b>
<ul>
<li>Diagnosed DNS resolution failures using dig and system logs</li>
<li>Verified reverse DNS lookups using PTR records</li>
 <li>Troubleshot network connectivity and interface issues using ip and ping</li>
 <li>Flushed DNS cache using resolvectl to validate changes</li>
 <li>Managed DNS and system services using systemctl</li>
 <li>Performed end-to-end connectivity testing between Linux server and Windows client</li>
</ul>





<h2>Screenshots</h2>

<b>Key Takeaways</b>
<ul>
<li>Strengthened understanding of DNS infrastructure and name resolution</li>
<li>Gained hands-on experience with Linux system administration</li>
 <li>Improved troubleshooting methodology for network and service-related issues</li>
 <li>Built practical skills aligned with NOC and entry-level system administration roles</li>
 </ul>

<b>Future Improvements</b>
<ul>
<li>Add DHCP service for dynamic IP assignment</li>
<li>Implement firewall rules (UFW) for network segmentation</li>
 <li>Expand to multi-server environment (web server, monitoring tools)</li>
 </ul>




<p align="center">
Network Diagram: <br/>
<img src="https://github.com/jasons559/Active-Directory-Home-Lab/blob/main/ADimages/Overview_Windows11_Windows_Server_UTM_MacM4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
BIND9 Configuration:  <br/>
<img src="https://github.com/jasons559/Active-Directory-Home-Lab/blob/main/ADimages/Domain_Controller_Setup.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Successful DNS Query: <br/>
<img src="https://github.com/jasons559/Active-Directory-Home-Lab/blob/main/ADimages/DNS_Configuration_Static_IPv4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Reverse DNS Query:  <br/>
<img src="https://github.com/jasons559/Active-Directory-Home-Lab/blob/main/ADimages/Windows_Client_Domain_Join.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />



</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
