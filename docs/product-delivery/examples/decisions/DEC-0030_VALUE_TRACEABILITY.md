# [DEC-0030] Trace work to customer/user value and operational learning

| Field | Value |
|---|---|
| **Type** | Product / Delivery |
| **Status** | Accepted |
| **Owner** | STAR Product Delivery leadership |
| **Decision date** | 2026-07-12 |
| **Effective date** | 2026-07-12 |
| **Review date / trigger** | Review after the first real Mission completes V1 and V2 |
| **Supersedes** | None |
| **Superseded by** | None |

## Context

Product, project and engineering activity can become internally focused when requirements, code, tests and releases are not connected to the customer or user problem that justified the work. The team also needs to learn from operational results after release rather than treating code completion as the outcome.

## Decision

Work and deliverables must remain traceable to customer or end-user value and to later operational evidence and learning.

The minimum delivery view therefore begins with the value need and ends with evidence, feedback or learning. Detailed artifacts remain linked rather than becoming the purpose of the process.

## Options considered

| Option | Benefits | Costs / risks | Why accepted or rejected |
|---|---|---|---|
| A. Manage delivery primarily through tasks and artifacts | Familiar and easy to count | Activity can be completed without proving value or operational success | Rejected as the primary model |
| B. Trace value need → Mission → work → release/operation → evidence/learning | Keeps purpose and outcome visible across teams | Requires explicit ownership, links and measurement | Accepted as the current candidate direction |
| C. Require a single comprehensive document for all traceability | Centralized view | High maintenance and cognitive load; likely to become stale | Rejected in favor of linked authoritative sources |

## Rationale and evidence

- Confirmed customer/end-user priority in `DEC-0015`.
- Confirmed need for team-readable progressive disclosure in `DEC-0010`–`DEC-0013`.
- Desk-tested against SmartQuote discount rules and a GateHub PSP connector in `10_MODEL_VALIDATION.md`.
- The model remains candidate until real-Mission validation is completed.

## Consequences

### Expected benefits

- Teams can explain why work exists and what outcome proves success.
- Release and operational evidence become part of completion.
- Customer-facing, product, engineering and operations teams share a common Mission view.

### Trade-offs and risks accepted

- Some outcome measures may be delayed beyond release.
- Links and ownership require maintenance.
- Not every task will directly map to an external customer; internal value receivers must still be explicit.

### Required follow-up work

- Complete V1 and V2 in `15_VALIDATION_PLAN.md` using a real active Mission.
- Test whether the Mission Brief is concise enough for all participant groups.

## Impact and relationships

- **Customers / users affected:** all value receivers represented by a Mission.
- **Products / capabilities affected:** SmartQuote, GateHub and future STAR products.
- **Missions / work items affected:** all material Product Delivery Missions.
- **Services / APIs / data affected:** linked according to Mission scope.
- **Teams / owners affected:** product, project, architecture, engineering, QA, AI, operations and governance.
- **Related decisions and artifacts:** `DEC-0015`, `DEC-0029`, `DEC-0031`, `11_FOUNDATION_CANDIDATE.md`, `templates/MISSION_BRIEF.md`.

## Validation

- **Success evidence:** a real Mission can be understood and executed across roles while preserving value and post-release evidence.
- **Failure / revisit trigger:** teams cannot identify the value receiver or evidence, or the traceability burden exceeds practical benefit.
- **Measurement owner:** Mission Owner with Product/Service Owner follow-through.
