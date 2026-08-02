# PDAP Architecture Readiness Gates

## Gate 0 — Phase 0 Evidence Gate

**Required evidence:** authoritative-source inventory; owners and freshness; Missing, Unknown, conflicting and superseded records; current Shared Foundation, SmartQuote and GateHub evidence; blocker and assumption candidates.

**Blocks only when:** authoritative source cannot be established, material authority conflicts cannot be safely resolved, or essential ownership is Missing.

**Allowed:** read-only inventory, evidence mapping, bounded interviews and assumption preparation.

**Prohibited:** technology approval, production architecture approval or development start.

**Approver:** Jason Lin.

## Gate 1 — Company / Shared Foundation Gate

**Required evidence:** company/shared capability boundary; core data ownership; Identity/Tenant/Security direction; cross-product dependencies; bounded technology baseline; repository structure and ownership; environment readiness; Git/PR/CI/CD baseline; testing baseline; secrets/configuration direction; observability/audit direction; deployment/rollback direction; post-start engineering owner; Approved Assumptions; ADR/RFC backlog; blocking-decision register.

A bounded technology baseline establishes a safe engineering boundary; it is not a final technology-stack freeze.

**Allowed:** bounded options, controlled Spikes, interface hypotheses and ADR/RFC preparation.

**Prohibited:** treating a Spike as engineering start or automatically authorizing product development.

## Gate 2 — SmartQuote Architecture Readiness Gate

**Required minimum package:** system context; domain boundaries; core data and system of record; component boundaries; API/integration boundaries; Identity/Tenant/security impact; deployment direction; critical NFRs; first delivery scope; out-of-scope; Shared Foundation dependencies; blocking decisions; Approved Assumptions; ADR/RFC backlog; readiness recommendation.

**Prohibited until passed and separately committed:** M1 Passed claim, M001 Committed, formal implementation or SmartQuote Delivery start.

## Gate 3 — GateHub Architecture Readiness Gate

**Required minimum package:** system context; domain boundaries; core data and system of record; component boundaries; API/integration; gateway/routing/connector boundaries; Identity/Tenant/security; deployment direction; critical NFRs; first delivery scope; out-of-scope; Shared Foundation and SmartQuote dependencies; blocking decisions; Approved Assumptions; ADR/RFC backlog; readiness recommendation.

GateHub must not automatically inherit SmartQuote product architecture decisions.

## Gate 4 — Cross-product Review Gate

**Required evidence:** shared capability ownership; duplicated capabilities; conflicting system-of-record claims; data ownership consistency; Identity/Tenant/Security consistency; API/event/integration conflicts; deployment and operational conflicts; critical NFR conflicts; irreversible decisions; remaining assumptions and ADR/RFC items; disposition for each material conflict.

Relevant specialists validate specific professional questions. Dorden is not the sole professional reviewer.

## Gate 5 — Product Commitment / Delivery Start Gate

**Required evidence:** applicable Architecture Gate disposition; Cross-product Review disposition; explicit Product Commitment; core delivery team; accountable delivery owner; repository and environment; CI quality controls; initial increment; test ownership; security/data disposition; open risks and assumptions; ADR/RFC backlog; delivery handoff; target start; rollback/recovery direction.

Only after explicit passage and Commitment may Allen enter execution coordination and formal development begin.

## Common failure and recovery

A failed or blocked Gate records the blocker, owner, evidence required, decision or closure date, recovery plan and revised forecast. Target dates alone never cause Gate passage.
