<h1>Home Data Center Lab</h1>


<h2>Description</h2>

<p>This project demonstrates the deployment and administration, of a virtual enterprise network environment, using Windows Server and Active Directory. The objective of this lab was to simulate a corporate IT infrastructure, by configuring a domain controller, implementing centralized authentication, managing users and organizational units, and applying security policies through Group Policy.
The environment includes a domain controller running Windows Server, and a domain-joined client machine running Windows 11 Pro. This active directory project, demonstrates core system administration tasks such as:domain configuration, DNS management, user administration, security policy enforcement, and troubleshooting domain connectivity issues.</p>

<h2>Network Architecture</h2>
<p>The lab environment was built using virtual machines running on an Apple Silicon MacBook Pro. The network was configured to simulate an internal enterprise LAN environment with static IP addressing and internal DNS resolution.</p>


| System    | Role        | Operating System |
|---------- |-------------| -----------------|
|DC01       |DomainController/DNS Server |Windows Server |
|WIN 11-Client| Domain Client| Windows 11 Pro|



<b>Network Configuration</b>
<ul>
<li>Domain Name: corp.local</li>
<li>Domain Controller</li>
<li>Domain Controller IP: 192.168.64.10</li>
 <li>Client IP: 192.168.64.10</li>
 <li>Internal DNS handled by the Domain Controller</li>
</ul>
<p>The environment simulates a simplified enterprise network, where authentication and policy enforcement are centralized through Active Directory.</p>

<h2>Domain Controller Setup</h2>

<p>A Domain Controller was deployed using Windows Server, and configured to host an Active Directory domain.</p>
<p><b>Key Steps Included:</b></p>
<ul>
<li>Installing the Active Directory Domain Services (AD DS) role</li>
<li>Promoting the server to a Domain Controller</li>
<li>Creating the domain corp.local</li>
<li>Configuring server networking with a static IP address</li>
<li>Renaming the server to DC01</li>
 </ul>
<p><b>Creating Organizational Units,(OUs) for departments such as:</b></p>
<ul>
<li>IT</li>
<li>HR</li>
<li>Sales</li>
 <li>Creating domain user accounts and administrative accounts</li>
  <li>Configuring shared folders for departmental file access</li>
 </ul>
This setup created the centralized authentication infrastructure for the lab environment.

<h2>DNS Configuration</h2>

<p>Internal name resolution was configured using the Domain Name System service running on the Domain Controller.</p>
<p><b>Key Configurations Included:</b></p>
<ul>
<li>Configuring the domain DNS zone for corp.local</li>
<li>Verifying name resolution using tools such as:</li>
<li>ping</li>
<li>nslookup</li>
<li>Configuring the Windows client machine to use the Domain Controller as its preferred DNS Server</li>
</ul>
DNS was essential for enabling domain authentication, and allowing the client machine to locate domain services.

<h2>Windows Client Domain Join</h2>

<p>A client system running Windows 11 Pro was deployed, and joined to the corp.local domain</p>
<p><b>Steps Include:</b></p>
<ul>
<li>Installing Windows 11 Pro in a virtual machine</li>
<li>Configuring network settings to use the Domain Controller DNS Server</li>
<li>Verifying the connectivity to DCO1</li>
<li>Joining the system to the Active Directory Domain</li>
<li>Loggin in using domain creditials</li>
</ul>
This allowed centralized user authentication, and demonstrated typical enterprise worktation configuration

<h2>Group Policy Implementation</h2>

<p>Security and system management policies were implemented using Group Policy</p>
<p><b>Policies configured in this lab include:</b></p>
<p><b>Password Policy</b></p>
<ul>
<li>Minimum password length</li>
<li>Password complexity requirements</li>
<li>Password history enforcement</li>
<li>Password expiration configuration</li>
 </ul>
<p><b>Account Lockout Policy</b></p>
<ul>
<li>Lockout threshold after failed login attempts</li>
<li>Automatic unlock duration</li> 
<li>Lockout counter reset timing</li> 
</ul>

<p><b>Device Security Policy</b></p>
<ul>
<li>Disabled removable USB storage devices, through Group Policy</li> 
</ul>
Policies were tested on domain-joined client using:"gpupdate /force"
This demonstrates centralized security policy enforcement across domain-joined machines

<h2>Troubleshooting Process</h2>
<p>During the implementation of this lab, I encountered, and resolved several technical challenges. Troubleshooting involved analyzing network connectivity, domain authentication failures, DNS resolution issues, and virtualization networking configurations.</p>

<p><b>Key Troubleshooting activities include:</b></p>
<ul>
<li>Diagnosing DNS resolution failures using ping, and nslookup</li>
<li>Resolving domain join failures</li>
<li>Password history enforcement</li>
<li>Addressing virtualization networking limitations between hypervisors</li>
<li>Reconfiguring static IP addressing</li>
<li>Resolving issues caused by Windows Home edition lacking domain join capabilities</li> 
<li>Validating Group Policy application on client systems</li> 
</ul>
This troubleshooting process provided hands on experience, with real-world system administration challenges, commonly encountered in enterprise environments.

<p><b>Skills Demonstrated:</b></p>
<ul>
<li>Active Directory Administration</li>
<li>Domain Controller deployment</li>
<li>DNS configuration and troubleshooting</li>
<li>Group Policy Management</li>
<li>Windows Server administration</li>
<li>Enterprise network troubleshooting</li> 
<li>Identity and access management</li> 
</ul>

<br />

<h2>Utilities Used</h2>

- <b>UTM Virtual Machine</b> 
- <b>VMware Fusion</b>
- <b>Macbook Pro M4</b>

<h2>Environments Used </h2>

- <b>Windows 11,</b>
- <b> Windows Server 2025</b>

<h2>Screenshots</h2>

<p align="center">
Overview(Windows Server+Windows 11 Pro): <br/>
<img src="https://github.com/jasons559/Active-Directory-Home-Lab/blob/main/ADimages/Overview_Windows11_Windows_Server_UTM_MacM4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Domain Controller Setup:  <br/>
<img src="https://github.com/jasons559/Active-Directory-Home-Lab/blob/main/ADimages/Domain_Controller_Setup.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
DNS Configuration (Static IPv4): <br/>
<img src="https://github.com/jasons559/Active-Directory-Home-Lab/blob/main/ADimages/DNS_Configuration_Static_IPv4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Windows Client Domain Join:  <br/>
<img src="https://github.com/jasons559/Active-Directory-Home-Lab/blob/main/ADimages/Windows_Client_Domain_Join.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Group Policy Security Hardening:  <br/>
<img src="https://github.com/jasons559/Active-Directory-Home-Lab/blob/main/ADimages/Group_Policy_Security_Hardening.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Troubleshooting Process:  <br/>
<img src="https://github.com/jasons559/Active-Directory-Home-Lab/blob/main/ADimages/Troubleshooting.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
