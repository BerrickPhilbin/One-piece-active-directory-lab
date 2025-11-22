<p align="center">
  <img src="https://i.imgur.com/CS2qwib.png" alt="Active Directory Logo" />
</p>

<h1>Active Directory — Server Deployment & Configuration</h1>

This guide documents the process of deploying and configuring an **Active Directory Domain Services (AD DS)** environment from start to finish.

---

<h2>🧰 Environments and Technologies Used</h2>

- Microsoft Azure / VirtualBox / VMware (Hypervisor or Cloud VM)  
- Windows Server (2019 / 2022)  
- Windows 10 / 11 (Client Machine)  
- Remote Desktop  
- Active Directory Domain Services (AD DS)  
- DNS  

---

<h2>🔄 Deployment Overview</h2>

- Step 1 — Preparing the Virtual Environment  
- Step 2 — Installing Windows Server  
- Step 3 — Configuring the Server & Network Settings  
- Step 4 — Installing Active Directory Domain Services  
- Step 5 — Promoting the Server to a Domain Controller  
- Step 6 — Creating Users & Testing Domain Join  

---

<h2>📝 Step 1: Preparing the Windows server VM</h2>

Set up your virtual machine or cloud server, allocate the appropriate resources (CPU, RAM, and storage), and ensure networking is configured so clients can reach the server.

<p align="center">
  <img src="https://i.imgur.com/xVQ8ZfZ.png" width="80%" alt="VM Setup" />
</p>

---

<h2>📝 Step 2: Preparing the Client VM</h2>

Install Windows Server on the VM. After installation, complete the initial setup and log into the machine for configuration.

<p align="center">
  <img src="https://i.imgur.com/rcZXjH0.png" width="80%" alt="Windows Server Installation" />
</p>

---

<h2>📝 Step 3: Configuring the Server & Network Settings</h2>

Assign a **static IP address**, configure the hostname, and verify network connectivity. A stable network configuration is required before installing AD DS.

<p align="center">
  <img src="https://i.imgur.com/D9ndNH0.png" width="80%" alt="Network Settings" />
</p>

---

<h2>📝 Step 4: Installing Active Directory Domain Services</h2>

Open **Server Manager**, add the **AD DS** role, and confirm installation. This prepares the system for promotion to a domain controller.

<p align="center">
  <img src="https://i.imgur.com/PKZijzt.png" width="80%" alt="Installing AD DS" />
</p>

---

<h2>📝 Step 5: Promoting the Server to a Domain Controller</h2>

Promote the server to a Domain Controller, create a new forest/domain, configure DNS, and complete the installation. The server will reboot.

---

<h2>📝 Step 6: Creating Users & Testing Domain Join</h2>

Use **Active Directory Users and Computers (ADUC)** to create organizational units (OUs) and user accounts.  
Test domain functionality by joining a Windows 10/11 client to the domain.

<p align="center">
  <img src="https://i.imgur.com/bS2nQE0.png" width="80%" alt="ADUC Setup" />
</p>

<p align="center">
  <img src="https://i.imgur.com/OlWCO0d.png" width="80%" alt="ADUC Setup" />
</p>

---

<h2>🎉 Conclusion</h2>

Your Active Directory environment is now fully configured. You can expand by adding Group Policies, additional servers, or administrative roles.

---
