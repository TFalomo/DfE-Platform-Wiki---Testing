# Tenants and Environments

## Resource-hosting tenants

Four Entra ID tenants host Azure resources:

| Tenant/environment | Purpose |
|---|---|
| Primary DfE `education.gov.uk` tenant | Corporate tenant containing Tier 1 and the strategic ELZ |
| SIP/CIP platform tenant | Flexible service-subscription model developed outside Tier 1 |
| FCS tenant | Inherited funding-service estate, mainly production/pre-production |
| CDS tenant | Inherited citizen/digital-service estate, mainly development/test |

Other Entra External ID or B2C tenants may support authentication scenarios but should not be described as Azure resource-hosting tenants unless verified.

## Consolidation principle

ELZ is the preferred destination for new services. Existing workloads should move when re-architecture, major change, supportability or risk provides a justified migration point. A blanket tenant move without business or technical benefit is not the default approach.

## Decision factors

- identity and B2B guest complexity
- corporate network dependencies
- application lifecycle
- security and compliance benefit
- cost and outage risk
- refactoring requirements
- operational ownership
- available migration funding.
