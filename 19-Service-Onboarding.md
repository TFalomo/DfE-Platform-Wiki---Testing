# Service Onboarding

## ELZ onboarding checklist

1. Confirm service owner, criticality, data classification and cost centre.
2. Request Dev/Test/Prod subscriptions and approved management-group placement.
3. Define Entra ID Reader, Contributor, owner and PIM approver groups.
4. Design core/spoke VNets, vWAN connectivity, IP ranges and expected traffic flows.
5. Confirm corporate DNS, private endpoints, Private DNS Zones and certificate needs.
6. Select approved IaC tool, GitHub/Azure DevOps repository and deployment identity.
7. Apply required tags, diagnostic settings, backup and Defender decisions.
8. Create monitoring, incident, change, restore and recovery runbooks.
9. Complete architecture/security review and test non-production connectivity.
10. Record dependencies, RPO/RTO, ownership and production acceptance evidence.

## Production entry criteria

- no unresolved critical security findings
- PIM and least-privilege access tested
- monitoring and alert ownership proven
- backup and restore tested
- DNS and certificate expiry monitoring enabled
- cost alerts configured
- rollback or roll-forward procedure approved
- architecture and dependency pages current.
