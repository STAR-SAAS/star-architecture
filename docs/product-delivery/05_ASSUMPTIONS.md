# STAR Assumptions and Working Hypotheses

**Version:** v0.1.1  
**Status:** Not confirmed architecture

| ID | Hypothesis | Confidence | Validation required |
|---|---|---:|---|
| ASM-001 | STAR's first practical foundation should be capability-oriented rather than tool-oriented. | Medium-high | Map one end-to-end Mission and show that capabilities remain stable while tools vary. |
| ASM-002 | A useful delivery loop may be expressed as need/value → Mission → work → delivery → operation/learning. | Medium | Run SmartQuote and GateHub examples and identify missing states. |
| ASM-003 | Mission is likely the primary cross-functional delivery container. | Medium | Define size limits, hierarchy, lifecycle and counterexamples. |
| ASM-004 | Work-centric views may be more useful than purely role-centric dashboards. | Medium | Conduct role walkthroughs; test people performing multiple work types. |
| ASM-005 | AI quality will depend heavily on current, authorized and relationship-aware context. | High | Prototype one AI development task using a structured context package and compare results. |
| ASM-006 | Stable IDs and explicit relationships can provide most early traceability without a dedicated graph database. | Medium-high | Implement links in Markdown/YAML for one Mission and measure retrieval quality. |
| ASM-007 | Progressive disclosure can reduce learning cost while preserving deep traceability. | High | Usability test executive, PM, developer, QA and Ops views. |
| ASM-008 | `STARSAAS/star-architecture` is the likely GitHub home for this foundation. | Confirmed | Resolved by `DEC-0032` on 2026-07-12. |
| ASM-009 | A generic Decision Record may cover product, business, architecture and governance decisions with a type field. | Medium | Compare with separate ADR/PDR/BDR/GDR templates on real decisions. |
| ASM-010 | STAR should eventually dogfood its own change, review, release and learning mechanisms. | Medium-high | Use the process for the first repository change and inspect friction. |

## Rule

An assumption becomes a decision only after evidence, review and explicit acceptance. It is moved by adding a new Decision ID; this file retains the historical assumption and its outcome.
