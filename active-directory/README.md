# Active Directory

## Overview

This section of the Enterprise Windows Server Home Lab documents the deployment and administration of Active Directory within a Windows Server 2025 enterprise environment.

Active Directory provides centralized authentication, authorization, and management for users, computers, security groups, and organizational resources.

Each topic below is documented in its own folder with step-by-step instructions, screenshots, and explanations.

---

# Topics

## 1. Installing Active Directory

Deploy Active Directory Domain Services (AD DS) and promote the server to the first Domain Controller.

**Folder**

```text
install-active-directory/
```

Topics covered:

- Installing AD DS
- Promoting the server to a Domain Controller
- Creating the homelab.local forest
- DNS installation
- Deployment verification

---

## 2. Organizational Units

Create an enterprise Organizational Unit (OU) structure for departments.

Topics covered:

- Creating department OUs
- Enterprise organization
- Administrative separation
- Preparing for Group Policy

---

## 3. Users and Security Groups

Create users and manage security groups following Microsoft's recommended best practices.

Topics covered:

- Creating user accounts
- Security Groups
- Group Membership
- Role-Based Access Control (RBAC)

---

## 4. Joining Computers to the Domain

*In Progress*

Topics covered:

- Joining Windows clients to Active Directory
- Domain authentication
- Computer accounts
- Domain logins

---

## Future Topics

The Active Directory section will continue expanding with additional enterprise administration topics including:

- Group Policy
- Password Policies
- User Management
- Computer Management
- Administrative Delegation
- Active Directory Troubleshooting

---

## Skills Demonstrated

- Windows Server Administration
- Active Directory
- Domain Controller Deployment
- Organizational Unit Design
- User Administration
- Security Group Management
- Enterprise Authentication
- DNS Integration
- Microsoft Best Practices

---

## Tools Used

- VMware Workstation Pro
- Windows Server 2025
- Server Manager
- Active Directory Users and Computers (ADUC)
- DNS Manager
