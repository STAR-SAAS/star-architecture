# STAR Information and Knowledge Governance — Candidate

| Field | Value |
|---|---|
| **Type / scope** | Governance candidate — authoritative sources and durable knowledge lifecycle |
| **Version / status** | v0.1.1 — Candidate; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | Product Delivery / Architecture maintainers |
| **Last reviewed** | 2026-07-12 |
| **Review trigger** | Actual tool/source map change, owner change, contradictory guidance, incident/audit finding or freeze proposal |
| **Authoritative working source** | This repository path in Draft PR #1; `main` only after approved merge |
| **Affects** | Product and engineering knowledge, active Missions, AI context, repository boundaries and all information-owning teams |
| **Supersession** | Supersedes the rejected idea that GitHub is the universal enterprise source of truth |
| **Access** | Public; sensitive source records remain in their authorized systems |

## Core rule

> Each information class has one authoritative source. Other tools may display or link to it, but should not create competing copies.

GitHub is authoritative for versioned product and engineering knowledge. It is not the authoritative system for every kind of enterprise information.

## Candidate authoritative-source map

| Information class | Candidate authoritative source | GitHub role |
|---|---|---|
| Product/engineering decisions, principles, standards and architecture baselines | GitHub Markdown / versioned repository | Authoritative |
| Source code, infrastructure as code, API/event schemas and versioned configuration | Relevant GitHub code repository | Authoritative |
| Mission summary and stable delivery baseline | GitHub Markdown linked to live work | Authoritative for the approved baseline, not minute-by-minute task state |
| Work items, assignments, dates, blockers and live delivery status | Issue/project tracking system | Link or summarize; do not duplicate live state manually |
| Customer, prospect, account and commercial relationship data | CRM | Link only, subject to access control |
| Support requests and customer service history | Service desk / support platform | Link relevant evidence; do not copy sensitive conversations unnecessarily |
| Runtime logs, traces, metrics, alerts and service health | Observability platform | Link dashboards and retained evidence |
| Deployment execution and current environment state | CI/CD, GitOps or deployment platform | Link release and deployment evidence |
| Incidents and active response coordination | Incident-management system | Link active record; store durable postmortem, decisions and learning where versioned knowledge belongs |
| Secrets, keys and credentials | Approved secrets manager | Never store secret values in Markdown or source history |
| Identity, access and authorization | Identity/IAM system | Document policy and ownership; do not duplicate live entitlements |
| Financial transactions and accounting records | Finance/ledger/ERP system | Link approved reports or controls where needed |
| Contracts, legal records and formal compliance evidence | Approved legal/compliance record system | Store references and non-sensitive guidance only |
| Email, chat, meetings and calendar | Communication/calendar systems | Treat as working input; extract material decisions and durable knowledge |
| Product usage and customer-behavior analytics | Analytics platform | Link measures and record interpreted evidence with source/date |
| AI context package | Dynamically assembled from authorized sources | Derived view; never becomes authoritative merely because AI used it |

The exact tools may change. The information class and authoritative-source rule should remain stable.

## Versioned knowledge lifecycle

```text
Candidate → Confirmed → Frozen (when required)
     ↓          ↓          ↓
  Rejected   Superseded  Superseded
                    ↓
                 Archived
```

- **Candidate:** plausible content still awaiting evidence, review or acceptance.
- **Confirmed:** accepted working knowledge or constraint.
- **Frozen:** approved stable baseline whose change requires an explicit superseding decision.
- **Rejected:** considered but not accepted; retained where useful to prevent repeated debate.
- **Superseded:** replaced by a newer item; remains traceable and points to the replacement.
- **Archived:** no longer active but retained according to legal, operational or historical needs.

## Minimum metadata for durable knowledge

Every material knowledge item should identify:

- ID and title;
- type and scope;
- owner;
- status;
- effective date and last review date;
- next review date or review trigger;
- authoritative source and related links;
- affected products, Missions, services or teams;
- supersedes / superseded by relationship;
- access classification where relevant.

Not every short team note needs this metadata. Apply it to material, reusable or decision-bearing knowledge.

## Review and expiry rules

Review is triggered by at least one of the following:

- scheduled review date;
- material product, architecture, regulatory or organizational change;
- incident or audit finding;
- owner change;
- linked system, API or product retirement;
- evidence that users or AI are receiving contradictory guidance.

An item with no active owner must not remain silently authoritative. It should be reassigned, downgraded, superseded or archived.

## Duplication rule

- Link to authoritative detail instead of copying it.
- A summary must state its source and current status.
- When a copy is unavoidable for legal or release reasons, label it as a snapshot with date/version.
- Chat or AI output is not durable knowledge until reviewed and recorded in the correct source.

## AI context rules

Every material AI context package should carry enough provenance to identify:

- source system and source link/ID;
- version, commit or timestamp;
- status and owner;
- access authorization;
- task scope and intended use;
- known conflicts or uncertainty.

AI-generated output remains a candidate contribution until the required automated checks and accountable human review are complete.

## Validation status

This is a candidate answer to `OQ-007` and `OQ-009`. It must be validated by mapping STAR's actual issue tracking, CRM, support, observability, CI/CD, identity, finance and legal systems. The principle should survive tool changes; the tool-specific map may not.
