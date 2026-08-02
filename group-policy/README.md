# Group Policy

## Overview

This section documents the implementation and administration of Microsoft Group Policy within a Windows Server 2025 Active Directory enterprise environment.

Group Policy provides centralized management for configuring Windows operating system settings, enforcing security policies, controlling user environments, and standardizing computer configurations across an Active Directory domain.

Each major topic is documented separately with objectives, explanations, screenshots, skills demonstrated, and lessons learned to mirror real-world enterprise infrastructure documentation.

---

## Table of Contents

1. [Creating and Linking Group Policy Objects](#1-creating-and-linking-group-policy-objects)
2. [Planned Documentation](#planned-documentation)
3. [Skills Demonstrated](#skills-demonstrated)
4. [Tools Used](#tools-used)
5. [Related Documentation](#related-documentation)

---

# Documentation Sections

## 1. Creating and Linking Group Policy Objects

**Status:** Complete

Create, configure, and deploy Group Policy Objects (GPOs) to manage user settings through Organizational Units (OUs). Validate successful policy deployment on a Windows client computer within the Active Directory domain.

**Documentation**

- [`create-and-link-group-policy/`](create-and-link-group-policy/)

Topics covered:

- Creating Group Policy Objects (GPOs)
- Linking GPOs to Organizational Units
- Configuring User Configuration policies
- Deploying Group Policy
- Forcing Group Policy updates
- Verifying policy application on Windows clients
- Basic enterprise policy management

---

## Planned Documentation

As the home lab expands, additional Group Policy administration topics will be documented.

### Security Policies

- Password Policies
- Password Complexity Requirements
- Account Lockout Policies
- Security Options

### User Environment Management

- Desktop Restrictions
- Control Panel Restrictions
- Start Menu Customization
- Folder Redirection
- Logon Scripts

### Enterprise Administration

- Drive Mapping
- Printer Deployment
- Software Deployment
- Windows Update Policies
- Security Filtering
- WMI Filtering
- Loopback Processing

### Troubleshooting

- Group Policy troubleshooting
- Policy inheritance
- Policy precedence
- Resultant Set of Policy (RSoP)
- GPResult analysis

---

## Skills Demonstrated

- Group Policy Object (GPO) Administration
- Organizational Unit (OU) Management
- Centralized Policy Deployment
- Enterprise User Management
- Active Directory Integration
- Client Policy Verification
- Windows Enterprise Administration
- Group Policy Troubleshooting

---

## Tools Used

- VMware Workstation Pro
- Windows Server 2025
- Windows 11
- Active Directory Domain Services (AD DS)
- Group Policy Management Console (GPMC)
- Group Policy Management Editor
- Command Prompt

---

## Related Documentation

Additional components of this enterprise lab include:

- Active Directory
- Networking
- DNS
- DHCP
- File Server
- Permissions
- Troubleshooting
