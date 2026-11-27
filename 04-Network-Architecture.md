# Network Architecture

## Current high-level model

```mermaid
flowchart LR
  O[DfE offices] --> PA[Prisma Access]
  R[Remote corporate laptops] -->|GlobalProtect| PA
  G[Gov Wi-Fi / guest path] -->|GlobalProtect where authorised| PA
  PA -->|Resilient service links| UKS[UK South vWAN hub]
  PA -->|Resilient service links| WEU[West Europe vWAN hub]
  UKS --> N1[Cloud NGFW]
  WEU --> N2[Cloud NGFW target pattern]
  N1 --> S1[Application spokes]
  N2 --> S2[Application spokes]
```

Offices do not use direct ExpressRoute as the primary model. The former BT MPLS and ExpressRoute design created a shared bottleneck and required numerous separately managed firewalls and gateways. Prisma Access now provides a common connectivity point for offices, remote users and Azure.

## Traffic-control layers

- **Prisma Access:** Central remote/office access and web security.
- **Azure vWAN:** Hub connectivity and route propagation.
- **Cloud NGFW:** Segmentation, internet control and east-west inspection.
- **WAF:** Layer 7 protection for inbound web applications.
- **Application controls:** NSGs, private endpoints, workload firewalls and identity controls.

## Architecture diagrams

Place approved exports from `Azure Landing Zone Wiki Diagrams-v0.4.vsdx` in `images/` and embed them here:

```markdown
![DfE holistic connectivity](images/dfe-holistic-connectivity.png)
![UK South secure hub](images/uk-south-secure-hub.png)
![West Europe migration](images/west-europe-migration.png)
```
