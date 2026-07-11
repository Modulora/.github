# Contributing to Modulora

Thank you for helping build Modulora. This policy applies across the Modulora GitHub organization unless a repository adds stricter instructions.

## Before contributing

- Read the repository README, PLAN, and CHECKLIST.
- Search existing issues and pull requests.
- Open an issue or RFC before large, cross-repository, security-sensitive, or breaking changes.
- Never include credentials, private component source, customer data, or vulnerability details in a public issue or pull request.

## Contribution workflow

1. Fork or branch from `main`.
2. Use a conventional branch name, such as `feat/component-search` or `fix/session-rotation`.
3. Keep changes focused and avoid unrelated cleanup.
4. Add or update tests and documentation.
5. Use Conventional Commits.
6. Sign off every commit under the Developer Certificate of Origin.
7. Open a pull request using the template.

## Developer Certificate of Origin

Modulora uses the [Developer Certificate of Origin 1.1](https://developercertificate.org/) instead of a CLA. By adding a `Signed-off-by` line, you certify that you have the right to submit the contribution under the repository's license.

```text
Signed-off-by: Your Name <you@example.com>
```

Create a signed-off commit with:

```bash
git commit -s -m "feat(scope): describe the change"
```

Every commit in the pull request must contain a valid sign-off. Do not sign for another contributor.

## Commit messages

Use Conventional Commits:

```text
feat(search): add compatibility filters
fix(auth): rotate session after factor enrollment
docs: clarify evidence semantics
```

Allowed types: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `chore`, `ci`, `build`, and `revert`.

## Pull requests

A pull request must explain:

- **What** changed.
- **Why** it is needed.
- **How** non-obvious decisions work.
- **Testing** performed.
- **Screenshots** for visible UI changes.
- **Security and privacy impact** for trust-boundary changes.

Draft pull requests are welcome for early feedback. Feature branches are squash-merged and deleted after merge.

## Security-sensitive changes

Changes to authentication, authorization, publishing, manifests, evidence, signatures, the installer, sandboxing, workflows, infrastructure, billing, private registries, or moderation require security-owner review. Include threat-model and rollback notes.

Report vulnerabilities privately using the instructions in [SECURITY.md](./SECURITY.md). Do not open a public vulnerability issue.

## AI-assisted contributions

AI tools may assist, but the human contributor remains responsible for correctness, provenance, licensing, security, tests, and the DCO sign-off. Do not submit generated code you do not have the right to license.

## Licenses

- `Modulora/modulora`: AGPL-3.0-only after the governance migration.
- `Modulora/spec` and `Modulora/cli`: Apache-2.0.
- `Modulora/cloud` and `Modulora/infra`: proprietary/private; contributions require explicit authorization.
- Creator component code retains its declared per-component license and is not relicensed by the platform.

## Conduct

Participation is governed by [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md).
