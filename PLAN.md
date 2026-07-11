# Organization Build Plan

> Repository: `Modulora/.github` · Status: approved planning baseline

## Mission

Make the Modulora organization safe, understandable, and contributor-ready. This repository owns organization identity, community health defaults, security-reporting guidance, repository policy documentation, and canonical brand assets.

## Ownership boundary

This repository owns:

- organization profile and public repository directory;
- issue forms, pull request templates, contribution/security/support defaults;
- organization-wide governance and repository policy documentation;
- canonical public brand assets and their usage terms.

It does not own application code, protocol schemas, CLI releases, production infrastructure, customer incidents, or private credentials.

## Dependencies and consumers

Every Modulora repository consumes these defaults. Security-sensitive repository-specific rules may be stricter but never weaker.

## Milestone 0 — Identity and brand

### Deliverables

- Publish the organization profile with the Modulora social header.
- Store canonical `social-header.png`, `profile-picture.png`, and `logo.svg` under `assets/brand/`.
- Document dimensions, intended use, and all-rights-reserved mark policy.
- Link public core, spec, and CLI repositories.
- Add website/docs links when domains are live.

### Acceptance

- Organization profile renders correctly on desktop and mobile GitHub views.
- Asset files preserve original dimensions and SVG contains no script/external executable content.
- Repositories reference canonical assets instead of uncontrolled duplicates.

## Milestone 1 — Community health

### Deliverables

- `CODE_OF_CONDUCT.md`.
- `CONTRIBUTING.md` with branch, commit, PR, DCO/CLA, testing, and security guidance.
- `SECURITY.md` with private vulnerability reporting, supported versions, response expectations, and scope.
- `SUPPORT.md` separating support, bugs, abuse, legal/takedown, and security channels.
- Issue forms: bug, feature, RFC, documentation, abuse/takedown pointer.
- Pull request template with what/why/how/testing/screenshots/security checklist.

### Acceptance

- Defaults appear in new/existing public repositories where not overridden.
- Security and abuse reports are directed away from public issues.
- Templates contain no promises the team cannot operationally meet.

## Milestone 2 — Teams and access policy

### Deliverables

- Teams: owners, maintainers, core, spec, cli, security, cloud, infra, moderation.
- Document least-privilege permissions and membership review cadence.
- Require organization 2FA; hardware-backed MFA for owners/privileged administrators.
- Add a second trusted owner before production and document recovery.
- Require access through teams rather than direct repository grants.

### Acceptance

- Team permissions match `Modulora/modulora/docs/github-organization.md`.
- No automation uses a broad personal access token.
- Quarterly membership/access review has an owner and checklist.

## Milestone 3 — Repository rulesets

### Deliverables

- Default-branch pull request requirement.
- CODEOWNERS approval for security-sensitive paths.
- Dismiss stale approvals; block force pushes/deletion.
- Required status checks once each repository has CI.
- Read-only default Actions token permissions.
- Protected release and deployment environments.
- Private vulnerability reporting enabled on public repositories.

### Acceptance

- A test branch cannot bypass configured protections.
- Fork PR workflows receive no secrets.
- Third-party Actions are pinned to immutable commit SHAs.
- Repository exceptions are documented and time-bounded.

## Milestone 4 — Package and integration ownership

### Deliverables

- Secure npm organization and exact/scoped package names.
- Enforce npm MFA and minimal maintainers.
- Configure trusted/OIDC publishing with provenance.
- Create the least-privilege Modulora GitHub App under organization ownership.
- Protect GitHub App key management and rotation documentation.

### Acceptance

- Package publication does not use long-lived npm tokens.
- GitHub App permissions are reviewed against actual endpoints.
- Compromise/revocation contacts and procedures are documented.

## Test contract

- Validate Markdown links and required community-health filenames.
- Scan documents and assets for secrets/active SVG content.
- Preview profile and templates before merge.
- Periodically test private vulnerability reporting and issue routing.

## Explicit non-goals

- Customer support records or active incident details.
- Production secrets, signing keys, or GitHub App private keys.
- Application-specific architecture decisions.
- Marketing campaigns beyond canonical organization identity.

## Definition of done

The organization foundation is complete when:

- brand/profile assets render correctly;
- community-health files and issue/PR templates are active;
- owner recovery, teams, 2FA, rulesets, CODEOWNERS, and Actions policy are operational;
- public vulnerability reporting is private and tested;
- npm and GitHub App ownership use least privilege and non-persistent credentials;
- every repository has a named owning team and consistent security baseline.

## Ongoing cadence

- Monthly dependency/workflow review.
- Quarterly owner/team/access review.
- Semiannual recovery and security-reporting exercise.
- Update repository links and status as projects launch.
