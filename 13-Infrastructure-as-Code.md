# Infrastructure as Code and Delivery

## Current state

Deployment practices are mixed across the estate:

- Terraform
- Bicep
- ARM templates
- Azure DevOps repositories and pipelines
- GitHub repositories and workflows
- manual Azure Portal deployment, particularly in older Tier 1 components.

## Strategic direction

Repositories, and potentially pipelines, are progressively moving toward GitHub Enterprise to use centrally purchased security capabilities such as secret scanning. Azure DevOps remains in use during the transition.

## Minimum engineering standard

- source-controlled infrastructure definition
- peer-reviewed pull requests
- environment separation
- remote and protected state for Terraform
- workload identity/federated credentials instead of long-lived secrets
- security and policy checks before deployment
- deployment logs retained
- rollback or roll-forward procedure
- no undocumented portal changes.

## Repository structure example

```text
/.github/workflows/
/infra/modules/
/infra/environments/dev/
/infra/environments/test/
/infra/environments/prod/
/docs/
CODEOWNERS
README.md
```
