# PDAP Shared Foundation and Product Gate Inputs

## Shared Foundation repository disposition

`STAR-SAAS/star-platform` is approved only as a Candidate Shared Foundation engineering repository.

```yaml
repository: STAR-SAAS/star-platform
disposition: Candidate — suitable for Shared Foundation engineering
authority_status: Unverified for engineering start
engineering_start_authorized: false
```

The repository still requires purpose, ownership, module-admission rules, branch and release model, CI/CD, environments, testing, secrets/configuration, observability, deployment/rollback and an engineering owner.

Product-specific SmartQuote and GateHub business code does not default into `star-platform`.

## Shared Foundation Gate 1 inputs

Bounded technology direction, not selection:

- prefer technologies supported by real team capability;
- prefer mature, maintainable and supported options;
- remain API-first and container-ready without mandating an orchestration platform;
- treat relational storage as a default candidate for core business records without choosing a database;
- use asynchronous integration only for evidenced decoupling, reliability or throughput needs;
- support independent deployment, Whitelabel, audit and rollback;
- avoid premature distributed-system complexity.

Minimum repository and engineering-start evidence:

- repository purpose and accountable owner;
- code ownership and module admission;
- product/shared boundary;
- branch, version and dependency rules;
- Local, Shared Development, Test/Integration, Staging and Production environment direction;
- configuration, secret, promotion, access, test-data and rollback boundaries;
- PR-based change control, builds, unit tests, lint/static checks, secret and dependency checks, artifact traceability and deployment approval;
- unit, API/contract, integration, security-sensitive, migration, smoke and rollback tests;
- externalized secrets, rotation ownership, access logging and least privilege;
- structured logs, correlation ID, Tenant context, health and business-failure signals, security audit and retention;
- repeatable deployment, traceable artifacts, schema-change strategy, health checks and rollback ownership;
- named post-start engineering owner before engineering begins.

Current owner candidates, not assignments:

- Ka Chen — Shared Foundation application engineering owner candidate;
- Eric — platform, infrastructure and operations owner candidate.

No task is assigned and no engineering start is authorized by these candidate roles.

## SmartQuote Gate 2 input map

| Gate input | Current state |
|---|---|
| System context | Candidate users and future CRM/Merchant Portal/partner integrations identified |
| Domain boundaries | Confirmed at Mission level |
| Merchant | minimum reference Candidate; complete ownership unresolved |
| Opportunity | Confirmed: one Merchant may have multiple Opportunities |
| Quote / Quote Version | Confirmed version retention |
| Pricing and Rule Center | Confirmed first-stage requirement |
| Frozen snapshots | Confirmed per Quote Version |
| Approval and permissions | Confirmed minimum flow |
| API | API-first requirement Confirmed; contracts Missing |
| Components | Missing |
| Systems of record | Quote/Version ownership Candidate; Merchant and reusable cost source unresolved |
| Identity/Tenant/Security | minimum shared boundary approved; product design Missing |
| Deployment | Whitelabel/independent-deployment constraint Confirmed; direction Missing |
| Critical NFRs | auditability, cost confidentiality, reliability and traceability Candidate |
| First scope / exclusions | Confirmed at Mission level |
| Repository/environment | Missing |
| ADR/RFC backlog | Candidate |
| Gate disposition | Not passed |

M1 remains not passed, M001 remains not Committed, and SmartQuote Delivery remains not started.

## GateHub Candidate authority baseline

Candidate business definition:

GateHub is a controlled capability for Merchant onboarding, bank/PSP application, payment-channel connection and related approval coordination. It organizes Merchant information, application materials, KYC/KYB state, bank/PSP onboarding, connector configuration references and approval evidence into traceable and auditable workflows.

Candidate first-stage scope:

- Merchant onboarding case and minimum Merchant reference;
- KYC/KYB checklist and evidence references;
- document-collection, review and approval state;
- bank/PSP application record;
- connector onboarding and readiness state;
- application and integration status tracking;
- accountable owner and audit evidence;
- API boundary for approved Merchant/channel availability.

Explicit first-stage exclusions:

- transaction processing and payment-routing execution;
- settlement, ledger and reconciliation;
- fraud decision engine;
- complete CRM;
- SmartQuote pricing and quote generation;
- universal document-management platform;
- autonomous AI KYC approval;
- unnecessary raw payment credentials;
- all-country regulatory automation.

Candidate ownership:

- Product/Accountable Owner: Jason Lin;
- Mission/Delivery, engineering, operations and compliance owners: Missing.

Boundary candidates:

- GateHub owns onboarding case and workflow state, not professional legal/compliance policy;
- connector scope initially covers registration, readiness, configuration metadata, credential references, bank/PSP state and certification evidence, not live transaction routing;
- GateHub may provide approved channel and onboarding availability to SmartQuote;
- SmartQuote must not read GateHub KYC documents or restricted personal data directly;
- pricing, cost and commercial terms do not automatically belong to GateHub.

GateHub authority state is Candidate. Gate 3 is not passed and GateHub Delivery has not started.