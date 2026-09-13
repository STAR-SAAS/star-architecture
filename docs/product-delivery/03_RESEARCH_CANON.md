# STAR Research Canon

**Version:** v0.1.0  
**Status:** Candidate Canon; not frozen  
**Source review date:** 2026-07-12

This file records what was researched, what was verified from primary/official sources, and the current STAR posture. "Adopt candidate" does not mean automatic full implementation.

## Source-verified candidates

| Method / standard | Verified purpose | Current STAR posture | Primary source |
|---|---|---|---|
| Domain-Driven Design (DDD) | Provides a framework and vocabulary for decisions in complex domain design. | Adopt strategic concepts selectively; do not turn all work into tactical DDD ceremony. | https://www.domainlanguage.com/ddd/ |
| Architecture Decision Records (ADR) | Captures a significant architectural decision, its rationale, trade-offs and consequences. | Adopt for architectural decisions; evaluate a generic Decision Record for non-architecture choices. | https://adr.github.io/ |
| C4 Model | Developer-friendly hierarchical architecture diagrams: system, container, component and code, plus supporting views. | Adopt as the default software architecture visualization approach. | https://c4model.com/ |
| ISO/IEC/IEEE 42010:2022 | Defines requirements for architecture descriptions, viewpoints and model kinds; it does not prescribe an architecting process. | Adopt its architecture-description principles; avoid claiming it defines the full delivery method. | https://www.iso.org/standard/74393.html |
| EventStorming | Collaborative workshop format for exploring complex business domains across disciplines. | Adopt when domain discovery or cross-team alignment warrants it; not mandatory for every change. | https://www.eventstorming.com/ |
| OpenAPI Specification | Language-agnostic description standard for HTTP APIs, usable by humans and machines. | Adopt for HTTP API contracts. Current official latest page showed OAS 3.2.0 during review. | https://spec.openapis.org/oas/latest.html |
| AsyncAPI Specification | Machine-readable, protocol-agnostic description of message-driven APIs. | Adopt when event/message APIs exist; do not force it on simple synchronous-only work. | https://www.asyncapi.com/docs/reference/specification/latest |
| OpenGitOps principles | Defines declarative, versioned/immutable, automatically pulled and continuously reconciled desired state. | Adopt later where infrastructure/deployment maturity justifies GitOps. | https://opengitops.dev/ |
| Google SRE | Connects engineering to the full software lifecycle and provides operational reliability practices. | Adopt reliability principles and practical mechanisms, scaled to STAR's product risk. | https://sre.google/books/ |
| Model Context Protocol (MCP) | Open standard for connecting AI applications to external systems, data, tools and workflows. | Track closely and use where it reduces proprietary AI integrations; security review required. | https://modelcontextprotocol.io/ |
| Agent2Agent (A2A) Protocol | Open standard for agent-to-agent communication and collaboration; current official site describes v1.0 and Linux Foundation governance. | Observe and prototype only when multi-agent interoperability becomes a concrete need. | https://a2a-protocol.org/latest/ |
| Backstage | Open-source framework for developer portals with catalog, templates and docs-as-code support. | Observe as a potential implementation option, not as the definition of STAR. | https://backstage.io/docs/overview/what-is-backstage/ |

## Discussed but requiring a dedicated source audit

| Method / standard | Preliminary posture | Audit needed |
|---|---|---|
| Team Topologies | Likely adopt selected team-boundary and interaction concepts. | Verify official definitions and fit to actual organization size. |
| arc42 | Likely use selected documentation sections. | Compare with ISO 42010 and avoid duplicate templates. |
| TOGAF | Partial use for governance/repository concepts only. | Verify current version and identify minimum useful subset. |
| BABOK | Partial use for business analysis and stakeholder/requirement thinking. | Validate against Product Management needs. |
| PMBOK | Partial use for risk, stakeholder and communication management. | Avoid project-heavy overhead. |
| SAFe | Limited reference for portfolio/capability language. | Validate whether any practice is needed at current scale. |
| Zachman | Classification reference only. | Determine whether it provides actionable value. |
| ISO/IEC/IEEE 15288 | Lifecycle reference candidate. | Confirm current edition and minimum mapping. |
| Docs as Code | Strong practice candidate, but scope must exclude dynamic operational/business data. | Define which knowledge classes are version-controlled. |
| Wardley Mapping | Strategy analysis candidate. | Test on build/buy/partner decisions. |
| Cynefin | Complexity-sensemaking candidate. | Validate whether it improves process selection. |
| OODA | Decision/feedback-loop reference candidate. | Test on incident and AI-agent workflows. |
| Knowledge Graph / ontology methods | Useful relationship and semantic concepts. | Do not select graph technology before a concrete retrieval problem exists. |

## Canon rules

A method enters the frozen Canon only when:

1. it solves a clearly stated STAR problem;
2. its authoritative source and current status are verified;
3. the minimum adoption profile is defined;
4. real SmartQuote or GateHub use demonstrates value;
5. team learning and operating cost are acceptable;
6. ownership and review date are assigned.

## Important correction

The earlier conversation occasionally used phrases such as "fully adopt" too quickly. This Canon intentionally replaces that language with **minimum, contextual adoption profiles**.
