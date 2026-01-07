# Microsoft Entra ID - User Types

| Type | Description |
|------|-------------|
| Cloud User | Pure cloud account, created directly in Entra ID |
| Guest User | External user invited via B2B |
| On-Prem User | Synced from on-prem Active Directory |
| Hybrid User | Synced + can sign in to both on-prem and cloud resources |

### Key Points
- External users can be invited as guests.
- Privileged Identity Management (PIM) and Access Reviews manage periodic access checks.
- Bulk user operations possible via Azure Portal or PowerShell (1-hour limit per operation).

# Microsoft Entra ID - Groups

## Types
| Type | Description |
|------|-------------|
| Security | Control access to apps/resources |
| Microsoft 365 | Collaboration (Teams, SharePoint) |

## Membership
- Assigned
- Dynamic (rules auto-assign users based on attributes)

## Group-Based Licensing
- Assign licenses at group level → automatically inherited by members
- Reduces manual errors
