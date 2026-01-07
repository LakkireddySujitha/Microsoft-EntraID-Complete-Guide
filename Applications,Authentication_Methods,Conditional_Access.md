# Microsoft Entra ID - Applications & Service Principals

## App Registrations
- Register any app (cloud or on-prem)
- Azure automatically creates a Service Principal

## Enterprise Applications
- Represents app instance for access management
- Assign users/groups
- Apply Conditional Access policies

## Managed Identities
| Type | Purpose |
|------|---------|
| System-assigned | Tied to one resource, auto-managed |
| User-assigned | Reusable, cross-resource |

- Used to access Key Vault, Storage, SQL, ARM APIs without secrets


# Microsoft Entra ID - Authentication Methods

| Method | How It Works | Use Case |
|--------|-------------|---------|
| Password Hash Sync (PHS) | Password hash synced to cloud, authentication in cloud | Cloud reliability, works even if on-prem is down |
| Pass-Through Auth (PTA) | Auth request sent to on-prem agent | Password stays on-prem, requires on-prem availability |
| Federation (AD FS) | Auth handled by AD FS | Custom auth / compliance requirements |
| Seamless SSO | Domain-joined device, single login | Reduce password prompts in corporate network |
| Passwordless | Microsoft Authenticator, FIDO2, Windows Hello | Phishing-resistant, modern authentication |

### Interview Tip
"PHS + Seamless SSO is most common; PTA or AD FS is for strict compliance; passwordless is modern & secure."


# Microsoft Entra ID - Conditional Access

## Advanced Controls

### Grant Controls
- Require MFA
- Require compliant device
- Require hybrid joined device
- Require approved client apps

### Session Controls
- Sign-in frequency
- Persistent browser
- App-enforced restrictions

### Report-only Mode
- Policy runs without enforcing
- Used to test impact before enabling

## Practical
Azure Portal → Entra ID → Security → Conditional Access → Policies  
Use risk signals from Identity Protection

### Interview One-liner
"Conditional Access enforces policies; Identity Protection provides intelligent risk signals."
