# Active Directory

## Overview

This section documents the deployment and administration of Microsoft Active Directory within a Windows Server 2025 enterprise environment.

Active Directory serves as the central identity management system for the lab, providing authentication, authorization, organizational structure, and security management for users, computers, security groups, and other network resources.

Each major topic is documented separately with objectives, explanations, screenshots, skills demonstrated, and lessons learned to mirror real-world enterprise infrastructure documentation.

---

## Table of Contents

1. [Installing Active Directory](#1-installing-active-directory)
2. [Organizational Units](#2-organizational-units)
3. [Users and Security Groups](#3-users-and-security-groups)
4. [Joining Computers to the Domain](#4-joining-computers-to-the-domain)
5. [Future Topics](#future-topics)
6. [Skills Demonstrated](#skills-demonstrated)
7. [Tools Used](#tools-used)
8. [Related Documentation](#related-documentation)

---

# Documentation Sections

## 1. Installing Active Directory

**Status:** Complete

Deploy Active Directory Domain Services (AD DS), install the first Domain Controller, create the Active Directory forest, and configure integrated DNS services.

**Documentation**

- [`install-active-directory/`](install-active-directory/)

Topics covered:

- Installing Active Directory Domain Services (AD DS)
- Promoting Windows Server to a Domain Controller
- Creating the **homelab.local** forest
- Installing and configuring DNS
- Verifying successful deployment

---

## 2. Organizational Units

**Status:** Complete

Design and implement an enterprise Organizational Unit (OU) structure to organize departments and prepare the environment for future Group Policy deployment.

**Documentation**

- [`organizational-units/`](organizational-units/)

Topics covered:

- Creating Organizational Units
- Creating department OUs
- Enterprise directory organization
- Administrative separation
- Preparing for Group Policy

---

## 3. Users and Security Groups

**Status:** Complete

Create user accounts and implement Global Security Groups following Microsoft's recommended identity and access management practices.

**Documentation**

- [`users-and-security-groups/`](users-and-security-groups/)

Topics covered:

- Creating user accounts
- Creating Global Security Groups
- Managing group membership
- Role-Based Access Control (RBAC)
- Enterprise permission management

---

## 4. Joining Computers to the Domain

**Status:** Complete

Join Windows client computers to the Active Directory domain, troubleshoot DNS-related connectivity issues, and verify successful authentication against the Domain Controller.

**Documentation**

- [`joining-computers-to-domain/`](joining-computers-to-domain/)

Topics covered:

- Troubleshooting DNS name resolution
- Configuring the Domain Controller as the client's DNS server
- Joining Windows clients to Active Directory
- Creating computer accounts
- Verifying domain authentication
- Logging in with domain user accounts
- Validating computer objects in Active Directory

---

## Future Topics

As the home lab expands, additional Active Directory administration topics will be documented.

### Identity Management

- Password Policies
- User Management
- Administrative Delegation

### Group Policy

- Group Policy Objects (GPOs)
- Department Policies
- Security Policies
- Software Deployment

### Computer Management

- Moving computer accounts into Organizational Units
- Domain-joined computer administration
- Remote administration

### Active Directory Maintenance

- User lifecycle management
- Organizational Unit administration
- Security Group administration

### Troubleshooting

- Active Directory troubleshooting
- Authentication issues
- DNS integration issues
- Group Policy troubleshooting

---

## Skills Demonstrated

- Windows Server Administration
- Active Directory Domain Services (AD DS)
- Domain Controller Deployment
- Organizational Unit Design
- Enterprise Directory Organization
- User Administration
- Security Group Administration
- Role-Based Access Control (RBAC)
- Domain Join Administration
- Client Deployment
- Enterprise Authentication
- DNS Troubleshooting
- Active Directory Troubleshooting
- Microsoft Active Directory Best Practices

---

## Tools Used

- VMware Workstation Pro
- Windows Server 2025
- Windows 11
- Server Manager
- Active Directory Users and Computers (ADUC)
- DNS Manager
- Command Prompt

---

## Related Documentation

Additional components of this enterprise lab include:

- Networking
- DNS
- DHCP
- Group Policy
- File Server
- Permissions
- Troubleshooting
