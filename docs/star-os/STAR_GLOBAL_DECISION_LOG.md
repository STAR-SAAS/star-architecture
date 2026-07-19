# STAR Global Decision Log

| Field | Value |
|---|---|
| **Version / status** | v0.1.1 — Active confirmed working decisions; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR OS governance maintainers |
| **Last reviewed** | 2026-07-19 |
| **Review trigger** | New global decision, supersession, cross-domain conflict or freeze proposal |
| **Scope** | All STAR work unless a decision states otherwise |
| **Access** | Public; sensitive governance records belong in approved private systems |

## Rules for this log

- Entries are append-only.
- A correction uses a new Decision ID and explicitly supersedes the earlier entry.
- A global decision is a working constraint, not automatically a frozen standard.
- Domain implementation details remain in the relevant domain records.

## Confirmed global decisions

| ID | Decision | Scope | Origin / basis |
|---|---|---|---|
| **GDEC-0001** | Every material task or document must be self-reviewed after completion; discovered issues are fixed before the next task begins. | Global | Explicit user requirement; previously reflected in Product Delivery `DEC-0001` |
| **GDEC-0002** | Material confirmed agreements must be proactively recorded in versioned Markdown; chat history is not the durable organizational memory. | Global | Explicit user requirement; Product Delivery `DEC-0020`–`DEC-0024` |
| **GDEC-0003** | A new or resumed STAR conversation must load global rules and relevant domain context before work begins; the user should not need to restate established rules. | Global | Explicitly accepted cross-conversation governance direction |
| **GDEC-0004** | Every material rule or decision must declare its scope and propagation targets. Narrower scopes must not silently override broader active rules. | Global | Explicitly accepted governance direction |
| **GDEC-0005** | STAR content must be concise, readable and progressively disclosed according to audience; detailed theory is not default front-line reading. | Global | Explicit user requirement; Product Delivery `DEC-0009`–`DEC-0013` |
| **GDEC-0006** | Before a multi-step batch, list the planned tasks; while working, provide timely status, next action, blocker and decision-needed updates. | Global | Explicit user requirement; Product Delivery `DEC-0033`–`DEC-0034` |
| **GDEC-0007** | Define the problem and review evidence before architecture or implementation; adopt or adapt mature methods before inventing replacements. | Global | Accepted research discipline; Product Delivery `DEC-0002`–`DEC-0006` |
| **GDEC-0008** | Design must start with customer/end-user value and proactively identify all affected internal, external, governance, AI and system stakeholders. | Global | Explicit user requirement; Product Delivery `DEC-0014`–`DEC-0019` |
| **GDEC-0009** | Do not claim completion, synchronization, validation, approval or freeze unless the relevant state has been verified. | Global | Confirmed integrity constraint; Product Delivery `DEC-0025`–`DEC-0027` |
| **GDEC-0010** | Routine reversible work within confirmed scope continues without repeated approval; leadership is asked only for strategic, broad, high-risk or genuinely preference-dependent decisions. | Global | Explicit/accepted working method; Product Delivery `DEC-0007`–`DEC-0008` |
| **GDEC-0011** | Missing owners, dates, permissions, customer facts or evidence must remain explicit gaps; examples and assumptions must not be promoted into facts. | Global | Accepted evidence discipline and repeated validation finding |
| **GDEC-0012** | STAR adopts the PDAP Founder-led Fast Track as the mandatory pre-development readiness covenant for Shared Foundation, SmartQuote and GateHub. Formal development requires the applicable Architecture Readiness and Product Commitment / Delivery Start Gates. Jason Lin and approved AI capabilities are the default pre-development executors; specialist participation is minimum-necessary and question-specific. Approved dates, blocker classes, assumptions, delay controls and detailed implementation rules are governed by the authoritative PDAP Master Program. | Global; direct propagation to PDAP, Shared Foundation, SmartQuote, GateHub, Command Desk and Product Delivery commitment boundaries | Leadership-confirmed DSP-001-021 |

## Propagation status

| Target | Current action |
|---|---|
| STAR global governance | Implemented in the Global Working Rules and Bootstrap Protocol |
| PDAP | Implemented in `docs/programs/pdap/`; publication and merge verification pending |
| Product Delivery | Existing Decision Log remains the domain record; future updates should link to these global decisions instead of duplicating them |
| STAR AI Governance | New conversation should bootstrap from this directory, then load AI Governance-specific records |
| Other STAR domains / Missions | Apply at the next conversation bootstrap or domain-governance update |

## Not yet global decisions

The following remain domain or candidate topics unless separately approved:

- final definition and commercial positioning of STAR OS;
- final Product Delivery hierarchy and meta-model;
- detailed AI account, tool, memory and technology-stack policies;
- product-specific architecture and implementation standards;
- numeric onboarding targets before real team validation.
