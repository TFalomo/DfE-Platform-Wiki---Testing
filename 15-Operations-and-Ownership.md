# Operations and Ownership

## Responsibility split

| Capability | Central/platform team | Business-service team |
|---|---:|---:|
| vWAN and hub connectivity | Accountable | Consulted |
| Prisma Access integration | Accountable | Consulted |
| Cloud NGFW platform | Accountable | Consulted |
| Azure Policy guardrails | Accountable | Consulted |
| Corporate DNS platform | Accountable | Responsible for requests/testing |
| Workload architecture | Consulted | Accountable |
| Workload IaC and deployment | Guardrail/support | Accountable |
| Application monitoring | Platform integration | Accountable |
| Workload backup and restore | Standards/support | Accountable |
| Service-specific paid Defender | Security guidance | Decision/funding owner |
| Cost optimisation | Reporting/guardrails | Accountable |

Replace generic roles with approved DfE team names and named service-owner groups before formal publication.

## Operational artefacts

Every production service should maintain:

- service record and ownership
- architecture diagram
- support hours and escalation
- monitoring and alerts
- dependency map
- backup/restore runbook
- DR/cyber-recovery plan
- change and deployment procedure
- cost and capacity review
- current risks and technical debt.
