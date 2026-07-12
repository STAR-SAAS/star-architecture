# STAR AI Work Governance — Candidate

| Field | Value |
|---|---|
| **Type / scope** | Governance candidate — AI work authority, controls and validation |
| **Version / status** | v0.1.1 — Candidate; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | Product Delivery / AI governance maintainers |
| **Last reviewed** | 2026-07-12 |
| **Review trigger** | Real AI-work finding, authority or risk change, security/privacy incident, conflicting decision or freeze proposal |
| **Authoritative working source** | This repository path in Draft PR #1; `main` only after approved merge |
| **Affects** | AI contributors, human reviewers/approvers and all Mission work that delegates material activity to AI |
| **Supersession** | None |
| **Access** | Public; secrets, restricted data and production credentials are excluded |

## Core rule

> AI may perform authorized work, but accountability remains with a named human owner.

AI access and autonomy should be proportional to impact, reversibility and the quality of available evidence.

## Candidate work levels

| Level | Typical AI work | Required control |
|---|---|---|
| **A0 — Assist** | Search, summarize, classify, explain or brainstorm without changing an authoritative source | Authorized context; material output is checked before reliance |
| **A1 — Propose** | Draft requirements, designs, code, tests, documentation or decisions | Named human reviewer before acceptance, merge or publication |
| **A2 — Execute reversible** | Run tests, update a working branch, prepare a draft PR, change sandbox data or perform a bounded tool action | Explicit task authorization, allowed tools/actions, logs, automated checks and human approval of the resulting change |
| **A3 — Execute high impact** | Production deployment, customer-facing communication, sensitive-data change, security action or financially significant operation | Named accountable human, explicit approval, least privilege, independent validation, rollback/recovery plan and complete audit trail |
| **A4 — Prohibited by default** | Autonomous executive/legal/compliance approval, bypassing controls, exposing secrets, irreversible destructive action or acting outside the authorized scope | Not allowed unless a later formally approved policy defines a safe exception |

The same task may move to a higher level when customer, security, privacy, compliance, financial or operational impact increases.

## Human-required boundaries

A named human must own or approve:

- Mission commitment and outcome accountability;
- product priority and customer promise;
- material architecture, risk and exception decisions;
- legal, compliance, security and financial acceptance;
- production release where impact is not low and fully reversible;
- use of sensitive or restricted data;
- final acceptance of material AI-generated knowledge.

AI can prepare evidence and recommendations for these decisions but does not silently inherit the authority.

## Minimum authorization for every material AI task

Before execution, identify:

1. **Task** — exact requested outcome and completion evidence.
2. **Scope** — products, repositories, environments, data and time boundary.
3. **Context** — current authoritative sources and known uncertainty.
4. **Allowed actions** — tools, writes, external communication and prohibited actions.
5. **Risk level** — A0–A4 plus customer, security, compliance, financial and operational impact.
6. **Reviewer / approver** — accountable human and required independent checks.
7. **Traceability** — logs, commits, artifacts, decisions and source provenance.
8. **Expiry** — when the authorization or context is no longer valid.

## Validation requirements

AI output is accepted only when the required evidence exists. Depending on the work, this may include:

- automated tests and policy checks;
- diff or artifact review;
- source and version verification;
- security/privacy review;
- human approval;
- sandbox or staged execution;
- production observation and rollback readiness;
- customer or user acceptance evidence.

Passing a model response review is not equivalent to validating the delivered outcome.

## Failure and escalation

AI must stop and escalate when:

- authoritative sources conflict;
- required context or permission is missing;
- requested action exceeds its authorization;
- impact or reversibility is uncertain;
- secrets or restricted data may be exposed;
- required checks fail;
- the requested outcome conflicts with a confirmed decision or policy.

The escalation should state what is known, what is uncertain, which action was not taken and who must decide next.

## Validation status

This document is a candidate answer to `OQ-011`. It must be tested on at least one AI product task, one code-change task, one QA task and one operational task before any work level becomes a frozen organizational policy.
