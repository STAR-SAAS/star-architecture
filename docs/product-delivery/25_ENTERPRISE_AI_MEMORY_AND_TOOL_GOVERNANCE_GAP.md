# STAR Enterprise AI Memory and Tool Governance — Public Gap Summary

| Field | Value |
|---|---|
| **Type / scope** | Public-safe governance summary — enterprise AI memory, tools, accounts, projects and technology controls |
| **Version / status** | v0.2.0 — Candidate; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | Product Delivery / Architecture / AI Governance / Security maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | AI governance decision, private-source selection, policy proposal, incident finding or material control change |
| **Authoritative working source** | Public summary in this Draft PR; detailed current-state evidence must use an approved private source |
| **Affects** | Company AI governance, project memory, technology standards and AI-enabled delivery |
| **Access** | Public summary only |

## Public/private boundary

This file records the governance problem and the non-sensitive control model. It deliberately does **not** contain:

- employee identities or account details;
- specific AI tools used by named people or teams;
- customer, project or security inventories;
- confidential architecture, source code or incident evidence;
- vendor-contract, billing or data-residency findings.

Those records belong in the private authoritative source for `⭐ STAR AI Governance`, which has not yet been selected.

## Why this domain exists

Enterprise AI use creates durable risks when company knowledge, project decisions, source code, technology choices or operating instructions exist only inside individual AI conversations, personal accounts or unregistered projects.

The governance objective is to make AI a controlled company capability rather than an unmanaged personal tool.

## Foundations already available

The Product Delivery work provides reusable candidates for:

- durable Decision Logs and Markdown-based working memory;
- Candidate, Confirmed, Frozen, Superseded and Archived states;
- one authoritative source per information class;
- owner, maintainer, review trigger and source metadata;
- AI context packages containing task, scope, sources, versions, authorization, reviewer, expiry and stop conditions;
- AI work levels A0–A4 with explicit human accountability;
- branch/PR-based reversible work and traceability;
- Mission, Decision Record and knowledge-metadata templates.

These are foundations only. They do not constitute company-wide AI governance by themselves.

## Governance capabilities still required

### 1. AI organization and accountability

- accountable AI Governance owner or body;
- security, privacy/legal, architecture/platform, procurement and business responsibilities;
- policy approval, exception and risk-acceptance authority;
- audit, incident and escalation ownership.

### 2. AI tool, vendor and account governance

- approved, restricted and prohibited AI tools/services;
- enterprise-managed identity, SSO/MFA, role-based access and offboarding;
- centralized billing, logs, retention and deletion controls;
- vendor security, privacy, intellectual-property and data-residency review;
- inventory of tools, models, agents, APIs and account types.

### 3. Memory and conversation governance

- company, project, work-session, AI-persistent and operational-evidence memory classes;
- data classification and allowed-input rules by tool/account type;
- retention, export, deletion, legal hold and offboarding requirements;
- promotion of durable decisions and knowledge from chats into authoritative sources;
- prevention of cross-project, cross-customer or unauthorized context leakage.

### 4. Project memory

Every AI-enabled project should eventually maintain a minimum company-owned memory package containing:

- business purpose, value receiver and accountable owner;
- approved repositories, architecture and technology profile;
- Decision Records, exceptions and current state;
- AI tools/models and authorized context sources;
- material instructions or agent configuration;
- dependencies, lockfiles, licenses and provenance;
- tests, security, release, operations, handover and retirement evidence.

### 5. Technology-stack governance

- approved technology profiles by project type;
- supported languages, frameworks, runtimes, databases and cloud services;
- reference architectures and starter repositories;
- version, patching and end-of-life rules;
- observability, security, deployment and support requirements;
- lightweight exception approval with owner, rationale, cost and exit plan.

Technology diversity is acceptable when intentional and owned. Unmanaged diversity is not.

### 6. AI-assisted software supply chain

- company-owned repositories for company projects;
- branch protection and accountable code review;
- tests, secret scanning, dependency/vulnerability and license checks;
- SBOM/provenance requirements where appropriate;
- controls for generated code, infrastructure and deployment assets;
- ownership and retirement of experiments or abandoned projects.

### 7. Measurement and continuous review

- AI usage, cost, quality and risk metrics;
- periodic review of tools, accounts, projects and vendor access;
- AI-related incident and exception records;
- evidence that employees understand and follow policy;
- review of whether AI-created assets remain maintainable and supported.

## Five memory classes

| Memory class | Purpose | Candidate authoritative location |
|---|---|---|
| **Company Memory** | Policies, standards, approved tools, global decisions and organization-wide learning | Governed company policy/knowledge repository |
| **Project Memory** | Requirements, decisions, architecture, code, tests, release and operations | Company-owned project repositories and linked systems |
| **Work-Session Memory** | Temporary human/AI conversation used to complete a task | Approved AI workspace; not authoritative by itself |
| **AI Persistent Memory** | Custom instructions, agents, retained files, vector stores and reusable context | Centrally governed enterprise AI workspace |
| **Operational Evidence** | Logs, incidents, metrics, deployments and support records | Observability, CI/CD, incident and support systems |

Core rule:

> A private AI conversation may support work, but it must not be the only place where company knowledge, source code, decisions or operating instructions exist.

## Immediate implementation candidates

1. Select a private authoritative repository/system for restricted AI Governance records.
2. Establish an AI Governance Charter, Decision Log, Open Questions, Work Status and Changelog.
3. Create private inventories for AI tools, accounts, projects, models, technology stacks and data classes.
4. Publish interim AI-use red lines and an incident/escalation path.
5. Require company-owned repositories and accountable owners for company software projects.
6. Define approved technology profiles and an exception process.
7. Define how durable project knowledge is migrated from personal AI workspaces into company sources.
8. Establish account provisioning, transfer and offboarding controls.

## Leadership decisions still required

- private authoritative repository/system;
- accountable AI Governance owner/body;
- approved enterprise AI tools and account model;
- data-classification and prohibited-input rules;
- default technology profiles and exception authority;
- project/account migration scope and enforcement sequence.

## Handoff

Continue the detailed implementation in `⭐ STAR AI Governance` using:

- `docs/star-os/handoffs/STAR_AI_GOVERNANCE.md`;
- the Global Working Rules and Bootstrap Protocol;
- an approved private source for restricted inventories and findings.

Do not repeat the user’s previously confirmed global working disciplines in the new conversation. Inherit them by Decision ID.