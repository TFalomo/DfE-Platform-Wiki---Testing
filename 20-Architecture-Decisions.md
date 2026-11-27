# Architecture Decisions

Use Architecture Decision Records (ADRs) for decisions that affect platform consistency or long-term support.

## ADR template

```markdown
# ADR-NNN: Decision title

- Status: Proposed / Accepted / Superseded
- Date:
- Owners:

## Context
What problem or constraint prompted the decision?

## Decision
What was decided?

## Consequences
What improves, what becomes harder, and what must teams do?

## Alternatives considered
What other options were evaluated and why were they rejected?

## Evidence and review date
Links to designs, risks, cost estimates and approval.
```

## Initial ADR candidates

- Prisma Access replacing office ExpressRoute as the central connectivity model
- UK South secure vWAN and Cloud NGFW as the strategic network pattern
- ELZ Dev/Test/Prod subscription separation
- PIM approval model by environment
- GitHub Enterprise strategic direction and Azure DevOps transition
- central Private DNS Zone and registration model
- criteria for paid Defender plans
- conditions for migrating legacy tenants/workloads into ELZ.
