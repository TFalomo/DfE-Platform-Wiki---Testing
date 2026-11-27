# West Europe Architecture

## Legacy design

West Europe was established before Azure UK regions were available. The original hub lacked integrated Cloud NGFW. It used:

- separate corporate-connectivity and internet-connectivity VNets
- Palo Alto firewall appliances
- extensive VNet peering
- user-defined routes
- Barracuda WAF services for inbound test and production applications.

## Target design

A West Europe vWAN hub with Cloud NGFW is intended to align the region with the UK South secure-hub model.

## Migration status

The meeting summary recorded:

- development migration complete
- test migration in progress
- production targeted for completion by March
- legacy connectivity VNets and firewalls to be decommissioned after migration.

> **Validate:** Record the target year and current completion status before publishing this as an operational commitment.

## WAF dependencies

Moving a workload region does not automatically move its WAF configuration. Application cutover plans must include DNS, certificates, WAF policy, backend pools, health probes and rollback.
