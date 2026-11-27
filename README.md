# DfE Azure Platform Wiki

A GitHub-ready technical wiki describing the DfE Azure platform, Enterprise Landing Zone, network architecture, identity, security, governance, engineering and operations.

## Import options

### GitHub Wiki repository
1. Enable **Wiki** under the repository **Settings > General > Features**.
2. Create the first wiki page in GitHub so the wiki Git repository exists.
3. Clone the wiki repository, whose URL normally ends in `.wiki.git`.
4. Copy all Markdown files from this package into the cloned wiki repository.
5. Copy the `images` directory and replace diagram placeholders with exported PNG/SVG versions of the approved architecture diagrams.
6. Commit and push.

### Normal GitHub repository
Commit this package to a `/wiki` or `/docs` directory. This is often preferable because it supports pull requests, branch protection, CODEOWNERS and review workflows.

## Source and validation status

This version consolidates the Azure platform overview meeting summary, prior DfE platform/DR material, and the architecture concepts in the Azure Landing Zone Wiki Diagrams. It deliberately omits presenter attribution.

Before treating it as authoritative, validate:
- West Europe production migration completion date and status
- current subscription counts
- GitHub Enterprise versus Azure DevOps policy scope
- mandatory paid Microsoft Defender plans
- private DNS automation status
- named service owners, RTOs and RPOs
- diagram classification and approval for publication
