# Backup, Disaster Recovery and Cyber Recovery

## Separate the outcomes

### High availability
Can the service tolerate failure of a VM, firewall, circuit, zone or component?

### Disaster recovery
Can it be restored after loss, deletion or corruption of a site, region, subscription or service?

### Cyber recovery
Can a trustworthy service be reconstructed after privileged identity, AD, Entra ID, PKI, policy or configuration compromise?

Replication alone is not a backup. Multiple compromised replicas do not provide cyber recovery.

## Required recovery record

| Field | Required information |
|---|---|
| Service criticality | Tier and business impact |
| Region/failure domain | Primary and secondary |
| Backup | Method, frequency, retention, immutability |
| RPO/RTO | Approved targets |
| Restore test | Date, result and evidence |
| Dependencies | Identity, DNS, PKI, network, Key Vault, pipelines |
| Recovery owner | Accountable team |
| Runbook | Version-controlled link |

Historic 24-hour RPO/RTO values for foundational services should be treated as baselines requiring owner validation, not automatically as current targets.
