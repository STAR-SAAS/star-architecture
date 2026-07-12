# STAR Decision Log

**Version:** v0.1.2  
**Status:** Active working log  
**Last consolidated:** 2026-07-12

## How to use this file

- Decisions are append-only. Corrections use a new decision that supersedes the old one.
- **Basis: Explicit** means the user directly stated the requirement.
- **Basis: Accepted** means the user accepted the proposal in the conversation.
- These decisions are confirmed working constraints, but are not automatically "frozen standards."

## Research and decision discipline

| ID | Decision | Basis |
|---|---|---|
| DEC-0001 | Do not rush. Each important step and document must be thoughtfully reviewed and validated before proceeding. | Explicit |
| DEC-0002 | Default to Research Mode until evidence is sufficient for Architecture Mode. | Accepted |
| DEC-0003 | Define the problem before researching or designing a solution. | Accepted |
| DEC-0004 | Use the sequence: research → architecture → design → implementation, with validation before freeze. | Accepted |
| DEC-0005 | Prefer evidence over opinion; distinguish facts, industry practice and STAR proposals. | Accepted |
| DEC-0006 | Adopt or adapt mature methods before inventing a STAR-specific replacement. | Accepted |
| DEC-0007 | Work in meaningful batches; do not stop after every small research item. | Explicit |
| DEC-0008 | Pause for the user only when a decision changes strategy, has broad architectural impact or presents two genuinely valid executive choices. | Explicit/Accepted |

## Communication and readability

| ID | Decision | Basis |
|---|---|---|
| DEC-0009 | Output should be concise; long repetitive philosophical narration is not useful. | Explicit |
| DEC-0010 | Ease of understanding and reading is a primary quality gate for STAR content. | Explicit |
| DEC-0011 | Use progressive disclosure: executive summary, team handbook, technical specification and research/reference layers serve different audiences. | Accepted |
| DEC-0012 | Front-line team members must not be required to understand the whole STAR theory before contributing. | Explicit/Accepted |
| DEC-0013 | Research material is not automatically a team-facing deliverable; it must be translated into actionable guidance. | Accepted |
| DEC-0033 | Provide timely, concise progress feedback while working on STAR tasks. Updates should name the current task, purpose, status, next action, blocker if any, and whether a user decision is needed. | Explicit |

## Stakeholders, customers and teams

| ID | Decision | Basis |
|---|---|---|
| DEC-0014 | Product Delivery design must consider architects, product managers, project managers, frontend, backend, QA, AI, operations and other relevant teams. | Explicit |
| DEC-0015 | Customer and end user are the most important stakeholders and must be considered from the beginning. | Explicit |
| DEC-0016 | The designer must proactively identify missing stakeholders instead of relying only on the roles named by the user. | Explicit |
| DEC-0017 | Stakeholder analysis must include external ecosystem participants, governance functions, support/operations, partner organizations and participating systems. | Accepted |
| DEC-0018 | Human and AI participants must both be included, with clear responsibility, authority and validation boundaries. | Accepted |
| DEC-0019 | Abstract proposals must be tested against real SmartQuote and GateHub scenarios before adoption. | Accepted |

## Knowledge and Markdown memory

| ID | Decision | Basis |
|---|---|---|
| DEC-0020 | Every confirmed material point must be proactively recorded in Markdown. | Explicit |
| DEC-0021 | Maintain separate records for confirmed decisions, open questions, assumptions, research and superseded ideas, plus a changelog. | Accepted |
| DEC-0022 | Review prior decisions before starting a new Mission or proposing a material design change. | Accepted |
| DEC-0023 | When a new proposal conflicts with history, name the affected decision ID and explicitly supersede or reject it. | Accepted |
| DEC-0024 | Chat history is working context, not the durable source of project truth. | Explicit/Accepted |

## GitHub and repository use

| ID | Decision | Basis |
|---|---|---|
| DEC-0025 | GitHub authorization does not cause automatic synchronization; publishing must be an explicit, verifiable action. | Confirmed fact accepted by user |
| DEC-0026 | GitHub is a primary authoritative repository for versioned product and engineering knowledge, not the universal source for all enterprise data. | Accepted |
| DEC-0027 | Do not claim that Markdown has been synchronized to GitHub unless the commit/push can be verified. | Derived from DEC-0020/0025; integrity constraint |
| DEC-0032 | Store this Product Delivery working-memory baseline in `STARSAAS/star-architecture` under `docs/product-delivery/`; introduce changes through a dedicated branch and pull request rather than placing the baseline directly on `main`. | Explicitly confirmed |

## Conversation and workstream boundary

| ID | Decision | Basis |
|---|---|---|
| DEC-0028 | Continue STAR OS Product Delivery and Foundation discussion in this conversation until a concrete Mission or sufficiently large specialist topic is split out. | Explicitly confirmed |

## Product Delivery direction

| ID | Decision | Basis |
|---|---|---|
| DEC-0029 | Architecture and documentation must support the Mission and the team; teams should not perform ceremony solely to satisfy the architecture. | Accepted direction |
| DEC-0030 | Work and deliverables should be traceable to customer/user value and later operational learning. | Accepted direction |
| DEC-0031 | STAR should optimize for role-relevant execution rather than showing every user the same dashboard, document set or theory. | Accepted direction |

## Not yet decisions

The following are intentionally **not** recorded as confirmed decisions: the final definition of STAR, the final Mission hierarchy, the final meta-model, "Work-Centric" as the sole design center, and the final names of proposed layers. They remain in `05_ASSUMPTIONS.md` or `02_OPEN_QUESTIONS.md`.
