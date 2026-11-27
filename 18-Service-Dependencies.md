# Service Dependencies

The dependency map is the operational centre of the wiki. It should answer: **If this component fails, what stops working, who recovers it, and what must be restored first?**

## End-user path

```mermaid
flowchart LR
  D[Managed device] --> LAN[LAN / Wi-Fi]
  LAN --> E[802.1X / PKI]
  E --> DHCP[DHCP]
  DHCP --> DNS[DNS / NTP]
  DNS --> AD[AD DS]
  AD --> FW[Routing / firewall]
  FW --> PA[Prisma Access]
  PA --> ENTRA[Entra ID / CA / MFA]
  ENTRA --> APP[Microsoft 365 / applications]
```

## Service dependency template

```text
Service:
Purpose:
Business owner:
Technical owner:
Tenant / management group / subscription / resource group:
Regions and failure domains:
Dependencies:
Consumers:
Authentication and privileged access:
Network path:
DNS and certificate dependencies:
HA design:
Backup and immutability:
RPO / RTO:
DR and cyber-recovery design:
Monitoring and alerts:
IaC repository and pipeline:
Runbook:
Risks and technical debt:
Last review / restore test:
```
