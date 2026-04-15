# 🔐 Active Directory Domain Lab

## 📌 Objective

The goal of this project is to design and implement a Windows Server Active Directory environment, simulating a real-world enterprise setup with centralized user management, security policies, and domain-based authentication.

---

## 🧱 Lab Environment

| Component  | Details              |
| ---------- | -------------------- |
| Hypervisor | VMware / VirtualBox  |
| Server OS  | Windows Server 2022  |
| Client OS  | Windows 10           |
| Network    | Internal Lab Network |

---

## 🖥️ Network Design

* Domain Controller: 192.168.1.10
* Client Machine: 192.168.1.20

*(Add your diagram screenshot here)*

---

## ⚙️ Implementation Steps

### 1. Install Windows Server

* Installed Windows Server 2022 on a virtual machine
* Configured static IP address

---

### 2. Configure Active Directory Domain Services (AD DS)

* Installed AD DS role
* Promoted server to Domain Controller
* Created domain: `homelab.local`

---

### 3. Create Organizational Units (OUs)

* HR
* IT
* Sales

---

### 4. User & Group Management

* Created users for each department
* Assigned users to security groups

---

### 5. Group Policy Configuration (GPO)

Implemented the following policies:

* Enforced password complexity
* Disabled USB storage access
* Configured desktop restrictions

---

### 6. Join Client to Domain

* Connected Windows 10 machine to domain
* Verified domain login functionality

---

## 🔍 Testing & Validation

* Successfully logged in as domain users
* Verified GPO policies applied correctly
* Tested access restrictions between departments

---

## 🐞 Problems Encountered & Fixes

### Issue 1: Client Could Not Join Domain

**Cause:** DNS misconfiguration
**Fix:** Set client DNS to Domain Controller IP

---

### Issue 2: GPO Not Applying

**Cause:** Policy not updated
**Fix:** Ran `gpupdate /force` and rebooted machine

---

## 📸 Screenshots

*(Add screenshots here)*

* AD Users and Computers
* Group Policy Management
* Domain login screen
* OU structure

---

## 🧠 Skills Demonstrated

* Active Directory Administration
* Group Policy Management
* Windows Server Configuration
* Troubleshooting & Issue Resolution

---

## 🚀 Key Takeaways

This project demonstrates my ability to deploy and manage a centralized identity system, enforce security policies, and troubleshoot common issues in a Windows Server environment.

---
