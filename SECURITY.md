# Security Policy

Security is a core product requirement for Modulora. We welcome responsible reports about organization repositories, packages, services, component publishing, account security, registry payloads, or supply-chain behavior.

## Report privately

Do not open a public issue for a vulnerability.

Use GitHub private vulnerability reporting in the affected public repository. If the affected repository has no private reporting form, use the [Modulora organization advisory form](https://github.com/Modulora/.github/security/advisories/new).

For a report, include when possible:

- affected repository, package, service, component, and version;
- impact and realistic attack scenario;
- reproduction steps or proof of concept;
- relevant logs or screenshots with secrets and personal data removed;
- suggested remediation;
- whether the issue is actively exploited or publicly known.

Do not access data that is not yours, degrade services, persist access, exfiltrate component source, or perform social engineering.

## Response targets

These are targets, not contractual SLAs:

- Initial acknowledgement: within 3 business days.
- Severity/triage update: within 7 business days.
- Remediation timeline: depends on impact, exploitability, and affected users.

We will coordinate disclosure when practical. We may publish an advisory and credit reporters who request attribution.

## Supported versions

Before the first public release, only the latest commit on `main` is maintained. After releases begin, supported versions will be listed in each repository.

## Security-sensitive areas

Reports are especially valuable for:

- account recovery, sessions, MFA, OAuth linking, and authorization;
- namespace ownership, GitHub App permissions, and publishing authority;
- manifest parsing, path traversal, symlink escapes, and installer behavior;
- signatures, digests, revocation, evidence, and release immutability;
- worker/sandbox isolation and network boundaries;
- private registry tenant isolation and token scope;
- workflows, package publishing, secrets, infrastructure, and dependencies.

## Safe harbor intent

When research follows this policy, avoids privacy/service harm, and is reported promptly, Modulora intends to work with the reporter in good faith and not pursue legal action solely for the research. This is a statement of intent, not legal advice or a waiver of third-party rights.
