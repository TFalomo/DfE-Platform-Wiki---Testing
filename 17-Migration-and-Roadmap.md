# Migration and Roadmap

## Workstreams

### West Europe network convergence
- complete test and production migration to vWAN/Cloud NGFW
- validate routes, DNS, WAF and monitoring
- decommission legacy connectivity VNets and firewalls only after rollback windows close.

### Tenant consolidation
- use ELZ for new services
- identify lifecycle-triggered migration candidates
- avoid tenant-only migration without measurable benefit.

### Private DNS automation
- establish central Private DNS Zones
- configure corporate conditional forwarding
- automate endpoint registration and lifecycle cleanup.

### Engineering standardisation
- clarify mandatory GitHub Enterprise scope
- define supported IaC tools and pipeline controls
- reduce portal-created infrastructure
- migrate repositories and pipelines in risk-based phases.

### Security baseline
- define when paid Defender plans are mandatory
- record exceptions and service funding
- standardise alert routing and posture reporting.

## Roadmap register

| Item | Owner | Target | Status | Evidence |
|---|---|---|---|---|
| West Europe production migration | Validate | Validate | Transition | Add link |
| Legacy firewall decommission | Validate | After migration | Planned | Add link |
| Private DNS automation | Validate | Validate | Planned | Add link |
| GitHub/Azure DevOps policy | Validate | Validate | Clarification required | Add link |
