# Static IPv4 Configuration

## Objective

Configure a Windows Server with a static IPv4 address to provide a consistent network identity for future enterprise services such as Active Directory and DNS.

---

## Environment

- Hypervisor: VMware Workstation Pro
- Operating System: Windows Server 2025
- Network Type: NAT (VMnet8)

---

## Initial Configuration

The server was initially configured to obtain its IPv4 address and DNS server automatically using DHCP.

The current configuration was inspected using:

```powershell
ipconfig /all
```

The following information was identified:

- IPv4 Address
- Subnet Mask
- Default Gateway
- DHCP Server
- DNS Server
- DHCP Status

---

## DHCP Scope Investigation

The VMware DHCP scope was reviewed before assigning a static address.

DHCP Range:

- Start: 192.168.130.128
- End: 192.168.130.254

To avoid potential IP conflicts, a static address outside of the DHCP scope was selected.

Assigned Static Address:

- IP Address: 192.168.130.10
- Subnet Mask: 255.255.255.0
- Default Gateway: 192.168.130.2
- Preferred DNS Server: 192.168.130.2

---

## Verification

The configuration was verified using:

```powershell
ipconfig /all
```

The output confirmed:

- DHCP Enabled: No
- Static IPv4 address assigned successfully

Network connectivity was verified using:

```powershell
ping 192.168.130.2
```

DNS name resolution was verified using:

```powershell
nslookup google.com
```

---

## Break/Fix Exercise

To reinforce the configuration process, the server was intentionally returned to DHCP.

The resulting configuration was investigated using PowerShell.

The server was then restored to its static IPv4 configuration without referencing previous notes.

After restoration, connectivity and DNS resolution were successfully verified.

---

## Skills Demonstrated

- Windows Server Administration
- Static IPv4 Configuration
- DHCP Investigation
- DNS Verification
- PowerShell
- Network Troubleshooting
- Break/Fix Troubleshooting

---

## Commands Used

```powershell
ipconfig /all

ping 192.168.130.2

nslookup google.com
```

---

## Lessons Learned

A server providing enterprise services should use a static IPv4 address instead of DHCP to ensure clients and services can reliably locate it.

Selecting a static address outside the DHCP scope helps reduce the risk of IP address conflicts with dynamically assigned devices.

Verifying changes using PowerShell commands after configuration is an essential part of the administrative process.
