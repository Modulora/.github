# GitHub Organization Checklist

## Organization security

- [ ] Require two-factor authentication for every member.
- [ ] Add a second trusted owner with hardware-backed MFA before production.
- [ ] Document owner recovery and emergency access.
- [x] Create least-privilege teams: maintainers, core, spec, cli, security, cloud, infra, moderation.
- [ ] Enable organization audit logging and security notifications.

## Community health

- [ ] Add default CODE_OF_CONDUCT.md.
- [ ] Add default CONTRIBUTING.md.
- [ ] Add default SECURITY.md with private reporting instructions.
- [ ] Add SUPPORT.md.
- [ ] Add issue forms for bugs, features, and RFCs.
- [ ] Add a pull request template with testing and screenshot sections.

## Repository policy

- [x] Require web-created commits to include DCO sign-off.
- [x] Protect default branches on public repositories. Private branch protection requires a paid GitHub organization plan and remains a launch blocker.
- [ ] Require pull requests, CODEOWNERS, status checks, and stale-approval dismissal.
- [x] Block force pushes and branch deletion on protected public branches.
- [x] Set Actions token permissions to read-only by default.
- [ ] Pin third-party Actions to commit SHAs.
- [ ] Protect package-publish and production environments.
- [x] Enable private vulnerability reporting for public repositories.

## Identity and packages

- [ ] Secure the npm organization and `modulora` package.
- [ ] Configure trusted/OIDC package publishing.
- [ ] Create the least-privilege GitHub App under Modulora ownership.
- [ ] Reserve verified domains and social handles after trademark review.
