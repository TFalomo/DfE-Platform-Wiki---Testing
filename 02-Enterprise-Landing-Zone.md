# Enterprise Landing Zone

## Purpose

The Enterprise Landing Zone is DfE's strategic model for securely hosting new services while allowing delivery teams to control application architecture.

## Standard subscription pattern

A service normally receives:

- a development subscription
- a test subscription
- a production subscription.

Each subscription sits beneath the appropriate management-group hierarchy and inherits policy and RBAC controls.

## Platform landing zones

Shared platform capabilities are separated into connectivity, identity and management concerns. Production services span UK South and West Europe where required. Application subscriptions consume shared services rather than duplicating platform components.

## Application landing-zone responsibilities

A service team normally owns:

- workload resources and architecture
- deployment pipelines and Infrastructure as Code
- application monitoring and incident response
- workload backup and recovery configuration
- service-level security and paid Defender decisions
- cost management and lifecycle.

## ELZ guardrails

Expected controls include:

- allowed regions and resource types
- permitted VM SKUs
- mandatory tags
- encryption requirements
- private networking and endpoint controls
- diagnostic settings
- RBAC through Entra ID groups
- PIM for elevated test and production access.
