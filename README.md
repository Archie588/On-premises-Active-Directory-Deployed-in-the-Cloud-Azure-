# On-premises-Active-Directory-Deployed-in-the-Cloud-Azure-

<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1: Install Micorosft Server 2022
- Step 2: Run the installation Wizard
- Step 3: Create Mydomain 
- Step 4: Set Group policy and Account Lockout Policy

<h2>Deployment and Configuration Steps</h2>

<p>
<img width="1002" alt="image" src="https://github.com/user-attachments/assets/e37eac2c-c8c8-4fd5-a428-d8af1f11bfb9" />

</p>
<p>
This steps shows the process installing Windows Server for Active Directory, the first essential step is to use the Server Manager's "Add Roles and Features Wizard" to install the Active Directory Domain Services (AD DS) role along with its required components. This process will automatically include necessary features such as Group Policy Management, Remote Server Administration Tools, Role Administration Tools, and various AD DS tools including PowerShell modules and administrative snap-ins. The wizard will display the installation progress and list all the components being installed, including AD DS Tools, Active Directory Administrative Center, and AD DS Snap-ins and Command-Line Tools, which are essential for managing your domain controller once the installation is complete.
</p>
<br />

<p>
<img width="864" alt="image" src="https://github.com/user-attachments/assets/f97b1511-99da-454a-8893-4b320d3825d6" />

</p>
<p>
The Windows Server Active Directory Domain Services installation has completed successfully, as indicated by the "Installation started on dc-1" progress bar and the comprehensive list of installed components including AD DS tools, Group Policy Management, and administrative utilities.
</p>
<br />

<p>
<img width="879" alt="image" src="https://github.com/user-attachments/assets/20e1745d-4f87-4cb8-a124-3ff7777f2c9a" />


</p>
<p>
Remote Desktop installated using Azure Virtual Machine environment that will let users log in and test the group policy assigned by the system Admin in the Active Directory Users and Computers tab where password policy and accout lockout policy under group policy management, under "Default Domain Policy" and "Account Lockout Policy" is configured.
</p>
<br />

<p>
<img width="1158" alt="image" src="https://github.com/user-attachments/assets/56bf61be-7a61-4657-b88c-d481dd9f29ed" />

</p>
<p>
This screenshot shows that Active Directory can be used to set Group Policy Management to centrally configure and enforce security settings, user permissions, and system configurations across an entire domain or organizational units. Administrators can create and modify Group Policy Objects (GPOs) like the Default Domain Policy, which contains various policy categories such as Account Policies, Account Lockout policies, and Kerberos policies as shown here. These policies automatically apply to users and computers within the specified scope of the Active Directory structure. The system allows IT administrators to maintain consistent security standards, such as enforcing password complexity requirements and managing account lockout settings. This centralized approach enables management of hundreds or thousands of domain-joined devices from a single location.
</p>
<br />

<p>
<img width="1216" alt="image" src="https://github.com/user-attachments/assets/acbae049-789c-48f0-90f3-e7d4c648a60e" />

</p>
<p>
The Active Directory Users and Computers allows systems Admins to configure password policy and account lockout policy using - group policy management, under "Default Domain Policy" and "Account Lockout Policy" as shown here on the screenshot.
</p>
<br />
