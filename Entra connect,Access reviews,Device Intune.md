# Microsoft Entra ID - Entra Connect (On-Prem Integration)

## Purpose
Connect on-prem Active Directory (AD) to Entra ID

## Features
| Feature | Description |
|---------|------------|
| Roles Needed | Global Admin (connect tenant), Domain Admin (read on-prem AD) |
| Methods | PHS, PTA, AD FS |
| App Proxy | For Kerberos/LDAP apps → Private Network Connector |
| Bulk Operations | Portal or PowerShell, 1-hour max per operation |

### Single Sign-On (SSO)
- Users sign in once
- MFA supported
- Re-registration possible

# Microsoft Entra ID - Access Reviews & PIM (Privileged Identity Management)

| Feature | Description |
|---------|------------|
| PIM | Just-in-Time admin access, time-limited |
| Access Reviews | Periodically check if users still need access |
| Automation | If no reviewer responds → conditions auto-enforced |

## Practical
Azure Portal → Entra ID → Identity Governance → PIM / Access Reviews  
Helps reduce unused privileges


# Microsoft Entra ID - Device Identity & Intune Integration

## Device Types
| Device Type | Description | Practical Click |
|-------------|------------|----------------|
| Azure AD Joined | Cloud-only device | Entra ID → Devices |
| Hybrid Azure AD Joined | On-prem + cloud | Entra ID → Devices → Join type |
| Azure AD Registered | BYOD | Entra ID → Devices |

## Device Compliance (Intune)
- OS version, encryption, antivirus, password policy
- Compliance signals used in Conditional Access policies

### Flow
1. Device enrolled in Intune → reports health
2. Entra ID queries compliance during login
3. Conditional Access grants or blocks access

### Interview Line
"Entra ID integrates with Intune to enforce device compliance for Conditional Access."

