# PR Broker

Exploring how AI agents can contribute to GitHub repositories while preserving human authority, security, and reviewability.

## Desired capabilities

- Agents can propose changes through pull requests.
- Humans retain control over approval, merge, and repository administration.
- Agents do not receive human administrator credentials.
- Repository owners can constrain agent authority.
- The solution is reusable across projects and organizations.

## Current direction

Start with GitHub Apps and GitHub-native repository protections. Establish experimentally which requirements these capabilities satisfy before introducing additional infrastructure.

Three candidate outcomes remain open:

1. A documented GitHub App configuration.
2. A GitHub App with a thin submission gateway.
3. A more capable PR broker where demonstrated needs justify it.

Prefer the simplest solution that meets the requirements.

## First experiment

Using a disposable repository, establish whether a GitHub App can:

- Create branches, commits, and pull requests.
- Enable independent human approval.
- Be prevented from directly modifying protected branches.
- Be prevented from merging, including after human approval.
- Respect restrictions on sensitive files and workflows.
- Support agent access without exposing privileged credentials.

Document the results, limitations, and remaining gaps.

## Project status

Exploratory development. No production-ready security implementation is available.

## Contributing

Questions, critiques, alternative approaches, experiments, documentation, and code contributions are welcome. Architecture decisions should remain open to challenge and be grounded in evidence.

## License

Apache-2.0.
