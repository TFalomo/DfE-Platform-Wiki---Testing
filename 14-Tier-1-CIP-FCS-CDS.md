# Legacy and Separate Azure Estates

## Tier 1

The original central DfE Azure environment used shared Production, Pre-production, Test, Development and Core subscriptions. Services shared VNets and centrally operated infrastructure. Internet-facing and backend workloads were historically represented as red and green zones.

Tier 1 remains heavily operated by central infrastructure teams and contains manually created legacy resources. It is not the default pattern for new services.

## SIP/CIP

This environment was created as a more flexible alternative to Tier 1. It introduced separate service subscriptions, PIM and centrally governed hub connectivity. Its separate tenant requires DfE users to use B2B guest identities and created additional identity complexity. Some platform components also retained dependencies on Tier 1 services.

## FCS and CDS

FCS and CDS originated from earlier organisational arrangements. They contain multiple subscriptions and VNets with varied access and operating practices. Treat them as inherited estates requiring workload-by-workload assessment rather than target reference architectures.

## Migration principle

Move services into new DfE ELZ subscriptions when lifecycle change or re-architecture creates sufficient benefit. Assess dependencies, identity, DNS, networking, data transfer, downtime, WAF, certificates and recovery before migration.
