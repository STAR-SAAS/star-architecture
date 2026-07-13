# STAR OS Global Decision Log

| Field | Value |
|---|---|
| **Version / status** | v0.1.0 — Active global working log; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR OS governance maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | New global decision, supersession, detected conflict, inheritance failure or freeze proposal |
| **Authoritative working source** | This file in the active Draft PR; `main` only after approved merge |
| **Supersession model** | Append-only; newer global Decision IDs explicitly supersede older decisions |

## Confirmed global decisions

| ID | Decision | Scope | Origin / basis |
|---|---|---|---|
| **GDEC-0001** | Confirmed STAR rules and decisions must be recorded in durable Markdown rather than relying on chat memory alone. | Global | Promoted from Product Delivery `DEC-0020`–`DEC-0024`; explicitly accepted |
| **GDEC-0002** | The user must not be asked to repeat or reconfirm a previously confirmed decision merely because work moved to a different STAR conversation. | Global | Explicit user requirement, 2026-07-13 |
| **GDEC-0003** | Every new or resumed STAR conversation must execute the Conversation Bootstrap Protocol before material work. | Global | Accepted implementation of `GDEC-0002` |
| **GDEC-0004** | Each material decision must record its scope, status, owner, authoritative source, propagation target and supersession relationship. | Global | Accepted governance requirement |
| **GDEC-0005** | A narrower workstream may specialize a broader rule, but may not silently contradict it; conflicts require an explicit exception or superseding decision. | Global | Accepted governance requirement |
| **GDEC-0006** | After every material task or document, perform a self-review, correct identified issues, update durable records and only then continue. | Global | Explicitly confirmed working discipline |
| **GDEC-0007** | Global rules apply to human and AI contributors; AI does not acquire approval authority merely by inheriting context. | Global | Promoted from Product Delivery AI governance direction |

## Reconfirmation policy

Existing decisions are inherited within their recorded scope. Leadership is asked again only when:

- a decision is proposed for change or supersession;
- scope is expanding beyond the original decision;
- new evidence, regulation, security or customer impact invalidates the earlier basis;
- an exception requires accountable risk acceptance;
- two or more valid alternatives require a new business preference.

Any such request must cite the affected Decision ID and explain the delta. It must never be phrased as though the prior decision did not exist.

## Relationship to domain logs

Domain, product and Mission logs keep their own decisions. A decision is copied here only when it is formally promoted to Global scope. The original Decision ID remains referenced for traceability.
