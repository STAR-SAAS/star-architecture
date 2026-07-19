# PDAP Assumption, ADR and RFC Register

## Approved temporary assumptions

| ID | Scope | Status | Expiry / review |
|---|---|---|---|
| AA-01 | Shared Foundation bounded start | Approved temporary | 2026-07-31 or Gate disposition |
| AA-02 | Product ownership by default | Approved temporary | 2026-07-31 or Gate 4 |
| AA-03 | SmartQuote internal API may precede external platform selection | Approved temporary | 2026-07-31 or Gate 2 |
| AA-04 | GateHub independent authority | Approved temporary | 2026-07-31 or Gate 3 |
| AA-05 | Technology-neutral observability outcomes for bounded Gate 1 use | Approved temporary | 2026-08-07 or RFC-PLT-007 approval, whichever occurs first |
| AA-06 | Tool-neutral CI quality-control outcomes for bounded Gate 1 use | Approved temporary | 2026-08-07 or RFC-PLT-004 approval, whichever occurs first |

Each assumption retains owner, scope, rationale, risk, validation trigger, expiry and reversal path.

AA-05 requires structured logs, correlation, health, failure visibility, redaction and minimum audit evidence. AA-06 requires repeatable build, unit test, lint/static check, secret check, dependency visibility, artifact identity and explicit pass/fail evidence. Neither assumption authorizes implementation, Gate passage, engineering start or an evidence-free merge.

## Candidate assumptions — not approved for use

- AA-07: product-local persistence first;
- AA-08: GateHub first slice excludes transaction routing as an assumption; the exclusion itself is already an approved first-stage boundary;
- AA-09: Merchant Identity may initially be a stable reference contract.

Candidate status does not authorize implementation or Gate passage.

## ADR backlog

- ADR-PDAP-001 Shared capability admission rule;
- ADR-PDAP-002 Merchant Identity ownership;
- ADR-PDAP-003 Merchant Commercial Profile ownership;
- ADR-PDAP-004 Tenant context and isolation;
- ADR-PDAP-005 Authentication versus product authorization;
- ADR-PDAP-006 Product audit semantics and shared audit envelope;
- ADR-PDAP-007 Product-local versus shared document metadata;
- ADR-SQ-001 Opportunity/Quote/Quote Version system of record;
- ADR-SQ-002 Quote snapshot immutability;
- ADR-SQ-003 Rule Center ownership;
- ADR-SQ-004 Channel-cost source and snapshot boundary;
- ADR-GH-001 GateHub onboarding and KYC boundary;
- ADR-GH-002 Connector ownership and lifecycle;
- ADR-GH-003 Credential-reference boundary.

## RFC backlog

- RFC-PLT-001 star-platform bootstrap;
- RFC-PLT-002 repository and module conventions;
- RFC-PLT-003 environment and promotion model;
- RFC-PLT-004 Git/PR/CI controls;
- RFC-PLT-005 testing baseline;
- RFC-PLT-006 secrets and configuration;
- RFC-PLT-007 observability and audit;
- RFC-PLT-008 deployment and rollback;
- RFC-SQ-001 SmartQuote API and errors;
- RFC-SQ-002 SmartQuote first delivery slice;
- RFC-GH-001 GateHub API and provider adapters;
- RFC-GH-002 bank/PSP application and certification evidence;
- RFC-GH-003 restricted-data and retention controls;
- RFC-PDAP-001 Whitelabel and independent-deployment constraints.

Backlog entries are not approved architecture, tools or implementation plans.