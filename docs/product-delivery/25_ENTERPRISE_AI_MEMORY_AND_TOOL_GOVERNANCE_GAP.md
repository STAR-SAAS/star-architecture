# STAR Enterprise AI Memory and Tool Governance — Gap Analysis

| Field | Value |
|---|---|
| **Type / scope** | Current-state and governance gap analysis — company, project and employee AI use |
| **Version / status** | v0.1.0 — Candidate; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | Product Delivery / Architecture / AI governance / Security maintainers |
| **Last reviewed** | 2026-07-13 |
| **Review trigger** | AI tool/account decision, employee onboarding/offboarding, new project, security/privacy incident, vendor change or policy proposal |
| **Authoritative working source** | This repository path in Draft PR #1; `main` only after approved merge |
| **Affects** | All employees, contractors, projects, code, customer/company data and AI-enabled work |
| **Access** | Public summary; sensitive inventories and incident details must remain restricted |

## Confirmed current-state input

STAR leadership reported that:

- employees have already used AI tools to build small software projects;
- projects use inconsistent technology stacks;
- employees use individual AI-tool accounts rather than centrally governed company accounts;
- AI use, project context and resulting assets are not yet under unified management.

This is a material organizational risk, not only a documentation issue.

## What the current Product Delivery work already covers

### Durable company/project memory

- Confirmed decisions are recorded in Markdown rather than left only in chat.
- Candidate, Confirmed, Frozen and Superseded states are separated.
- GitHub is the working authoritative source for versioned product and engineering knowledge.
- High-impact knowledge now has owner/maintainer, review trigger and authoritative-source metadata.
- A central Knowledge Review Register identifies which files require continuing review.

### AI task memory and context

- AI tasks can carry explicit scope, source versions, allowed actions, reviewer, uncertainty, expiry and stop conditions.
- AI context packages are derived views; they do not become authoritative merely because an AI used them.
- A1/A2/A3 candidate work levels separate proposal, reversible execution and high-impact execution.
- Human accountability remains explicit for acceptance, release, legal/compliance, security, financial and customer commitments.

### Reversible engineering governance

- AI documentation work has been performed on a dedicated branch and Draft PR.
- Git history, Decision Records and validation evidence provide traceability.
- Missing facts are recorded as blockers instead of being invented.

## What is not yet governed

### 1. Company-level AI management

Missing controls include:

- a company AI policy and acceptable-use standard;
- a complete inventory of AI tools, accounts, agents, APIs, models and AI-enabled projects;
- an approved AI service/provider list;
- enterprise-managed accounts, SSO/MFA, role-based access and centralized billing;
- employee/contractor onboarding, transfer and offboarding controls;
- vendor security, privacy, intellectual-property and data-residency assessment;
- central audit, incident reporting and policy-exception management;
- ownership for AI governance, security, legal/privacy, architecture and procurement decisions.

### 2. Employee-to-AI conversation memory

The company has not yet defined:

- which information may be entered into which AI tool;
- whether source code, customer data, credentials, contracts, financial data or internal architecture may be uploaded;
- when chat history or persistent memory must be disabled;
- retention, export, deletion and legal-hold rules;
- how valuable decisions or project knowledge move from a private chat into an authoritative project repository;
- how personal AI histories, custom instructions, agents, files and vector stores are transferred or deleted when an employee leaves;
- controls against cross-project or cross-customer context leakage;
- whether AI vendors may use submitted content for service improvement under each account type and contract.

### 3. Project memory

Projects do not yet have a mandatory minimum memory package containing:

- business purpose, owner and customer/user value;
- approved architecture and technology stack;
- Decision Records and exceptions;
- repositories, environments and deployment ownership;
- AI tools/models used and authorized context sources;
- prompts/instructions or agent configuration that materially affect output;
- dependencies, lockfiles, licenses and software bill of materials;
- test, security, release and operational evidence;
- handover, support and retirement information.

Without this package, project knowledge remains trapped in individual chats and accounts.

### 4. Technology-stack governance

STAR has not yet established:

- approved default stacks by project type;
- supported languages, frameworks, runtimes, databases and cloud services;
- version support and patching rules;
- reference architectures and project starter templates;
- an exception process for using another stack;
- ownership and maintenance expectations for every technology choice;
- compatibility, observability, deployment and security requirements;
- an end-of-life and migration policy.

Technology diversity is not automatically bad, but unmanaged diversity creates lasting maintenance and security cost.

### 5. AI-assisted software supply chain

Not yet implemented:

- mandatory company-owned repositories for every project;
- branch protection and code-review rules;
- dependency, secret, license and vulnerability scanning;
- SBOM and provenance requirements;
- test and security gates for AI-generated code;
- approved package registries and dependency sources;
- source-code ownership and third-party-code attribution checks;
- controls for generated infrastructure, deployment scripts and credentials;
- inventory and retirement of abandoned AI-built projects.

### 6. Measurement and incident handling

The company does not yet have:

- AI use metrics by team, project, tool and risk class;
- an AI-related incident channel and response process;
- monitoring for sensitive-data leakage or unauthorized tools;
- periodic review of AI projects, accounts and vendor access;
- quality/security comparisons between AI-generated and human-generated changes;
- evidence that governance controls are understood and followed by employees.

## Risk assessment

| Risk | Current severity | Why |
|---|---|---|
| Company data or code entered into unmanaged personal AI accounts | High | STAR cannot centrally enforce access, retention, deletion, contractual or offboarding controls |
| Project knowledge trapped in employee AI histories | High | The company may lose rationale, prompts, context and operating knowledge when a person or account disappears |
| Unmanaged technology-stack proliferation | High | Security patching, hiring, maintenance, deployment and support become fragmented |
| Shadow AI / shadow IT projects | High | Projects may lack owner, repository, testing, security, support and retirement controls |
| Credentials or sensitive information exposed to AI tools or generated code | Critical when present | Can create direct security, privacy, customer and operational impact |
| Unreviewed AI-generated dependencies and code | High | Introduces vulnerability, licensing, provenance and maintainability risk |
| No enterprise audit trail | High | STAR cannot reliably reconstruct what tool, model, context or person produced a consequential outcome |
| Vendor/account lock-in | Medium-high | Valuable organizational memory and workflows may remain inside individual vendor accounts |

## Immediate containment candidate

Before a full program is designed, STAR should consider these minimum controls:

1. Require every software project to be registered with owner, purpose, repository, stack and current status.
2. Require company-owned GitHub repositories for company work; prohibit source code existing only in AI chat or personal storage.
3. Publish an interim rule that secrets, credentials, customer data, regulated data and confidential contracts must not be entered into unapproved AI accounts.
4. Inventory all AI tools and account types currently used by employees and contractors.
5. Select a small approved enterprise AI-tool set with company-managed identity, access, retention and offboarding controls.
6. Define one default technology stack per common project type, with a documented exception path.
7. Require human review, automated tests, dependency/secret scanning and ownership before AI-generated code is deployed.
8. Export durable project decisions, architecture and operating knowledge from private chats into the project repository.
9. Assign accountable owners for AI governance, architecture/platform standards, security/privacy and procurement/vendor review.
10. Do not delete or disable existing employee accounts until project knowledge and access dependencies have been inventoried and safely migrated.

## Target governance model

A practical first model should separate five memory classes:

| Memory class | Purpose | Authoritative location |
|---|---|---|
| **Company memory** | Policies, standards, approved tools, risk decisions and organization-wide learning | Governed company repository / policy system |
| **Project memory** | Requirements, decisions, architecture, code, tests, release and operations | Company-owned project repositories and linked systems |
| **Work-session memory** | Temporary employee/AI conversation used to complete a task | Approved AI workspace; not authoritative by itself |
| **AI persistent memory** | Custom instructions, agents, files, vector stores and retained context | Centrally governed enterprise AI account/workspace |
| **Operational evidence** | Logs, incidents, metrics, deployments and support records | Observability, CI/CD, incident and support systems |

The core rule is:

> Private AI conversation memory may support work, but it must not become the only place where company knowledge, source code, decisions or operating instructions exist.

## Decisions still required

This document does not choose vendors or mandate a final technical stack. Leadership decisions are still needed for:

- accountable AI governance owner/body;
- approved enterprise AI tools and prohibited uses;
- company data-classification and AI input rules;
- default technology stacks and exception authority;
- project inventory and migration scope;
- employee-account migration and offboarding policy;
- enforcement level and rollout sequence.

## Current conclusion

STAR has built a useful **project-document, decision, context and AI-task governance foundation**, but it has **not yet built company-wide AI management, employee conversation-memory governance, account governance or technology-stack governance**.

The reported current state should therefore be treated as a new high-priority governance workstream, not as a minor addition to Product Delivery.