# STAR Role-View Desk Walkthrough

**Version:** v0.1.0  
**Status:** Desk-validation evidence; not a real participant test  
**Mission used:** GateHub PSP Connector example  
**Purpose:** Check whether each participant can understand the Mission and identify the information needed for action without reading the full research repository.

## Result summary

The one-page Mission view is sufficient for **orientation**, but not yet for **execution**. The main gaps are missing authoritative names, dates, dependencies, approvals, current-state links and evidence—not missing theory or additional document layers.

## Participant walkthrough

| Participant | What the current brief explains | What is still required for real action |
|---|---|---|
| **Customer / Merchant** | Expected payment coverage and operational value | Supported markets/methods, launch date, onboarding impact and pilot acceptance path |
| **Leadership / Sponsor** | Why the connector matters and major risk areas | Priority, target outcome, commercial case, accountable owner and decisions requiring escalation |
| **Product Manager / Owner** | Candidate scope, value and measures | Actual customer evidence, precise exclusions, rollout cohort and enduring Product Owner |
| **Project / Delivery Manager** | Main dependency categories and workstreams | Named owners, dates, external certification plan, blockers and milestone sequence |
| **Architect / Tech Lead** | Canonical model, idempotency, security and failure concerns | Current architecture links, existing decisions, provider contract and explicit technical constraints |
| **Backend Engineering** | Authentication, mapping, webhooks, retries and persistence work | Provider specification, repositories, environments, data contract and acceptance examples |
| **Frontend / Portal** | UI is needed only when configuration or operations require it | Confirmed portal impact, user permissions, states and design source |
| **QA / Quality Engineering** | Positive, negative, contract, resilience and regression needs | Sandbox access, certification cases, test data, environments and release gate |
| **AI Team / Agent** | AI may draft mappings, tests and documentation under review | Authorized task, context sources, allowed tools, reviewer, expiry and stop conditions |
| **DevOps / SRE / Operations / Support** | Secrets, deployment, alerts, rollback and incident needs | Environment inventory, alert thresholds, runbook owner, on-call path and support readiness |
| **Security / Risk / Compliance / Legal / Finance** | Due diligence, data handling and commercial obligations matter | Jurisdictions, data classification, contracts, approval owners and retained evidence |
| **Partner / PSP** | External API, credentials, certification and support are dependencies | Named contacts, service commitments, certification dates and escalation path |

## Findings

1. **Why / What / Who / Now / Evidence** remains a useful first-view structure.
2. Generic role names are not enough for execution; committed Missions need named accountable parties or linked team ownership.
3. `Now` must show a timestamped current state or link to the authoritative work tracker.
4. Evidence must identify its source, version/date and owner.
5. A stakeholder category should be explicitly marked **Not affected** rather than silently omitted.
6. Customer-facing views should hide internal implementation detail while preserving delivery date, impact and acceptance information.
7. AI views require explicit context, authorization and review boundaries beyond the ordinary contributor view.

## V4 validation status

**Desk walkthrough:** Complete.  
**Real participant comprehension test:** Not started.

The desk walkthrough supports the current design but does not prove usability. V4 remains open until representative participants use a real active Mission Brief and answer the validation questions in `15_VALIDATION_PLAN.md`.
