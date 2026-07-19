# Git / GitHub / Codex Access Verification Baseline

| Field | Value |
|---|---|
| Verification date | 2026-07-19 |
| GitHub account | `STARSAAS` |
| GitHub App organization installation | `STAR-SAAS` |
| Classification | Public-safe tooling access baseline |
| Scope | Access verification only; no permission, policy or governance change |

## User-verified local Windows evidence

The following evidence was provided by Jason Lin and is recorded as user-verified local evidence:

- Windows GitHub CLI authentication is active.
- The local token includes `repo`, `read:org` and `workflow` scopes.
- Local Windows `gh` authentication and Codex/cloud workspace authentication are separate environments.

This repository record does not independently inspect or reproduce the local Windows credential state.

## Connector-verified cloud evidence

Verified through the connected GitHub App on 2026-07-19:

- authenticated GitHub login: `STARSAAS`;
- GitHub App installation account: `STAR-SAAS`;
- connector access currently includes:
  - `STAR-SAAS/star-architecture` — Admin;
  - `STAR-SAAS/star-ai-governance` — Admin;
  - `STAR-SAAS/star-platform` — Admin;
  - `STAR-SAAS/star-domains` — Admin.

The originally reported two-repository list was narrower than the live connector installation scope and is therefore not retained as the current authoritative connector-access statement.

## Operating boundary

- Each Codex or connected task must explicitly load or resolve the intended repository before branch or file operations.
- Local Windows authentication does not automatically authenticate a separate cloud/Codex runtime.
- Connector visibility or Admin permission does not authorize repository, permission, policy or governance changes.
- Every write still requires task-specific scope and authorization.
- This record does not modify repository permissions, GitHub App installation scope, branch controls, policies or governance roles.

## Freshness

Reverify when any of the following changes:

- authenticated GitHub account;
- token scopes;
- GitHub App installation account or repository selection;
- repository permission level;
- local versus cloud execution environment;
- organization ownership or access policy.
