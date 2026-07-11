# GitHub Organization Checklist

## Organization security

- [ ] Require two-factor authentication for every member.
- [ ] Add a second trusted owner with hardware-backed MFA before production.
- [ ] Document owner recovery and emergency access.
- [ ] Create least-privilege teams: maintainers, core, spec, cli, security, cloud, infra.
- [ ] Enable organization audit logging and security notifications.

## Community health

- [ ] Add default CODE_OF_CONDUCT.md.
- [ ] Add default CONTRIBUTING.md.
- [ ] Add default SECURITY.md with private reporting instructions.
- [ ] Add SUPPORT.md.
- [ ] Add issue forms for bugs, features, and RFCs.
- [ ] Add a pull request template with testing and screenshot sections.

## Repository policy

- [ ] Apply default-branch rulesets to every repository.
- [ ] Require pull requests, CODEOWNERS, status checks, and stale-approval dismissal.
- [ ] Block force pushes and branch deletion.
- [ ] Set Actions token permissions to read-only by default.
- [ ] Pin third-party Actions to commit SHAs.
- [ ] Protect package-publish and production environments.
- [ ] Enable private vulnerability reporting for public repositories.

## Identity and packages

- [ ] Secure the npm organization and `modulora` package.
- [ ] Configure trusted/OIDC package publishing.
- [ ] Create the least-privilege GitHub App under Modulora ownership.
- [ ] Reserve verified domains and social handles after trademark review.
