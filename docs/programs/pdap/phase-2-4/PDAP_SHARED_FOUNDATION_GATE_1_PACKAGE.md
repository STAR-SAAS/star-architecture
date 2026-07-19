# PDAP Shared Foundation Gate 1 Package

## Status

- Recommendation: Recovery required.
- Gate 1: not passed.
- Engineering start: not authorized.
- Target 2026-07-27 remains At risk.

## Capability boundary

Shared Foundation is engineering-foundation-first. A capability enters Shared Foundation only when at least two products have a stable common need, semantics and lifecycle are compatible, shared ownership/versioning/operations are explicit, and sharing materially reduces duplication, operational risk or irreversible conflict.

Product capabilities remain product-owned by default. Premature general workflow, rule, Merchant, document, integration, microservice or shared-database platforms are prohibited without evidence.

## Candidate shared scope

- repository bootstrap and module conventions;
- Git, PR and merge controls;
- environment and promotion conventions;
- secrets and configuration integration;
- logging, metrics, tracing and audit-envelope conventions;
- deployment and rollback mechanics;
- dependency and OSS governance;
- common ADR, RFC and documentation structure;
- identity adapter, tenant propagation and authorization-enforcement primitives;
- API versioning, errors and correlation conventions;
- webhook, connector-lifecycle, document-metadata and notification primitives when stable reuse is proven.

## Bounded technology baseline

This package defines outcomes only. It does not select a language, framework, database, cloud, CI vendor, secrets manager, observability vendor, deployment topology or message broker.

Required outcomes are API-first, tenant-aware or explicitly tenant-neutral, secure-by-default, testable, observable, rollback-capable, traceable, maintainable, compatible with independent deployment and Whitelabel, and reversible where uncertainty remains.

Patterns requiring specific evidence before introduction include default microservices, event sourcing, active-active multi-region, service mesh, Kubernetes, custom identity provider, custom workflow engine, custom rule language, polyglot persistence, distributed transactions and unrelated shared databases.

## Candidate repository baseline

`STAR-SAAS/star-platform` remains a Candidate Shared Foundation repository. It is empty and not engineering-ready.

Candidate ownership:

- Accountable owner: Jason Lin;
- Application engineering owner candidate: Ka Chen;
- Platform/infrastructure/operations owner candidate: Eric.

These are not assignments or engineering authorization.

Minimum bootstrap candidate:

```text
README.md
CODEOWNERS
CONTRIBUTING.md
SECURITY.md
docs/architecture/
docs/adr/
docs/rfc/
docs/operations/
docs/standards/
foundation/
platform/
contracts/
tests/
scripts/
.github/pull_request_template.md
.github/workflows/
config/examples/
CHANGELOG.md
```

Each admitted module must record consuming products, reason for sharing, owner, contract, compatibility policy, tests, release model, deprecation path and reversal/extraction plan.

## Environment and control baseline

Candidate environments are Local, Shared Development, Test/Integration, Staging and Production. Before engineering start, ownership, configuration source, secret boundary, promotion, test-data handling, production access, rollback and recovery must be explicit.

Minimum engineering-control outcomes include PR-based change, traceable build/artifact, unit/contract/integration tests, lint/static analysis, dependency and vulnerability checks, secret scanning, deployment approval, health checks, rollback evidence, structured logs, correlation, tenant context, audit events, alert ownership and redaction.

AA-05 and AA-06 remain Candidate. These outcomes do not approve final observability or CI controls.

## Remaining blockers

| Blocker | Class | Owner | Evidence required | Recovery |
|---|---|---|---|---|
| Repository empty | Technical readiness | Jason Lin | approved bounded bootstrap | preparation only |
| Post-start owner unassigned | Authority | Jason Lin | explicit ownership | hold start |
| Environment/CI/tests absent | Technical/recovery | Jason Lin | executable minimum controls | no product work |
| Secrets/deployment/rollback unverified | Security/recovery | Jason Lin | minimum handling and recovery evidence | no production access |

## Recommendation

Recovery required. This is a preparation recommendation only and does not pass Gate 1 or authorize engineering.