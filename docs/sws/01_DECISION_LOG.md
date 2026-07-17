# SWS-001 · Decision Log

| Field | Value |
|---|---|
| **Version / status** | v0.2.3 — Active confirmed working decisions; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-17 (Asia/Singapore) |
| **Authoritative working source** | Draft PR #2 working branch plus DSP-001-018 child Draft PR record version until approved merge |
| **Scope** | SWS-001 · STAR Workspace Specification |

## Authority note

- Decision basis may be leadership-confirmed before the corresponding record version is merged.
- Entries introduced or corrected in child Draft PRs are proposed record versions until merged into the Draft PR #2 branch.
- After that merge, they become part of the Draft PR #2 working baseline; they remain not frozen and do not enter `main` unless Draft PR #2 is separately merged.

## Log rules

- Entries are append-only.
- Corrections use a new Decision ID and explicitly preserve or supersede the prior decision.
- Confirmed working decisions are not automatically approved or frozen standards.
- Tool-specific implementation details remain Candidate until verified in actual use.

## Decisions

| ID | Decision | Status | Scope | Basis / note |
|---|---|---|---|---|
| **SWS-DEC-001** | STAR Workspace uses a scope-governed, record-backed and context-driven platform model. Context is a runtime derived view; authoritative records remain in declared source systems. | Confirmed working direction; not frozen | SWS-001 | Accepted during SWS architecture review |
| **SWS-DEC-002** | The minimum information model consists of Scope, Actor, Capability, Activity, Record and Context Package, with Typed Relationship as a structural primitive. Artifact is a Record subtype; Actor and Capability remain separate. | Confirmed working direction; not frozen | SWS-001 | Accepted during core-object review |
| **SWS-DEC-003** | Every non-global Scope has one governance parent; cross-scope relationships use typed links. Rules may propagate downward, but membership, access, capabilities, records and context do not automatically inherit. | Confirmed working direction; not frozen | SWS-001 | Accepted during Scope Model review |
| **SWS-DEC-004** | Authorization separates Actor, Principal, Scope-bound Role Assignment, provider-neutral Capability and conditional Grant. Material capability defaults to deny; AI execution retains named human accountability. | Confirmed working direction; not frozen | SWS-001 | Accepted during authorization review |
| **SWS-DEC-005** | Launch STAR Command Center as a separate Project with only `⭐ STAR Command Desk`; use it only for intake, prioritization, routing, portfolio status and feedback. Professional execution remains in professional Projects. | Confirmed launch direction; implementation incomplete | SWS-001 / STAR Command Center | Explicitly confirmed by the user; Project and Chat reported created |
| **SWS-DEC-006** | `docs/sws/command-center/STAR-PORTFOLIO-STATUS.md` in `STARSAAS/star-architecture` is the authoritative portfolio-coordination ledger during the pilot. It is not authoritative for professional detail. | Confirmed working implementation decision; not frozen | SWS-001 / STAR Command Center pilot | Established by the authority-source task on 2026-07-14 |
| **SWS-DEC-007** | The Command Center pilot covers only SWS-001, STAR AI Governance and Mission-001 SmartQuote Foundation. No existing conversations are migrated or deleted during the pilot. | Confirmed launch direction | STAR Command Center pilot | Explicitly confirmed by the user |
| **SWS-DEC-008** | The operating loop is Dispatch → Execute → Report Back → Verify → Update Status → Feedback. Cross-project status must not rely only on chat memory. | Confirmed launch direction | STAR Command Center pilot | Explicitly confirmed by the user |
| **SWS-DEC-009** | Weekly Planning, Monthly Review, Dashboard and other management conversations are not created until actual usage proves a concrete need. | Confirmed launch direction | STAR Command Center pilot | Explicitly confirmed by the user |
| **SWS-DEC-010** | Every material STAR conversation uses a scope and ownership Contract, Routing Gate, lifecycle state and durable handoff/closure rules; the correct Project, conversation and mode are stated proactively. | Leadership-confirmed basis; proposed record version in PR #3; not frozen | All STAR conversations | Confirmed user requirements in DSP-001-004 |
| **SWS-DEC-011** | Chat, Work and Codex are selected by dominant work type. A brief mismatch warning is required, but authority remains in declared records and named humans. | Leadership-confirmed basis; proposed record version in PR #3; not frozen | STAR conversation execution | Confirmed user requirements in DSP-001-004 |
| **SWS-DEC-012** | GitHub is durable structured organizational memory, not a raw chat archive. Material decisions, status and evidence synchronize to GitHub while noise and sensitive data are excluded. | Leadership-confirmed basis; proposed record version in PR #3; not frozen | STAR organizational memory | Additional confirmed requirement in DSP-001-004 |
| **SWS-DEC-013** | Scope-level `CONTEXT_PACKAGE.md`, `ACTIVE_DECISIONS.md` and concise `WORK_STATUS.md` form the default runtime set. Loading is incremental by branch, required-file version and freshness metadata; whole-repository and full-history loading are not default. | Leadership-confirmed basis; proposed record version in PR #3; not frozen | Runtime context loading | Additional confirmed requirement in DSP-001-004 |
| **SWS-DEC-014** | The repository containing the SWS-001 portfolio ledger was subsequently transferred from `STARSAAS/star-architecture` to `STAR-SAAS/star-architecture`. The portfolio-ledger governance intent of SWS-DEC-006 remains active; only the repository-location identity is corrected, and the original confirmed decision remains historically visible. | Leadership-confirmed repository-state correction; proposed record version in PR #3; not frozen | SWS-001 / STAR Command Center pilot | Repository transfer verified after SWS-DEC-006; does not silently rewrite SWS-DEC-006 |
| **SWS-DEC-015** | Leadership approves the pre-start role matrices, controlled role-overlap exception, candidate locations and safety boundaries for SWS Pilot Packages A, B and C. Package A uses the existing private `STAR-SAAS/star-ai-governance` repository with Internal-only classification and no raw Confidential/Restricted data; Package B uses the approved Pilot Candidate Alias and M001 package paths; Package C uses the approved Command Desk context paths and Safe Ledger Update method. Allen Liao may hold maintainer and execution-owner roles for these three Packages only until Pilot closure, while Dorden remains the independent professional reviewer. These approvals do not start any Package, create any file, change access, update the Ledger, activate automation or authorize SmartQuote Delivery. | Leadership-approved startup conditions; implementation Missing; not a Pilot start authorization | SWS Pilot Packages A, B and C | DSP-001-015; approved by Jason Lin; overlap expires at Pilot closure and is reviewed on Package completion, role/access change, material finding or Pilot closure |
| **SWS-DEC-016** | Leadership confirms the GitHub identity bindings and the next-stage preparation controls for SWS Pilot Packages A, B and C. The normal publishing model remains Robin Koh through `rkoh-star`, with Allen Liao as human execution owner, Dorden as independent professional reviewer through `zhuangdongdong`, and Jason Lin as report-back approver through `STARSAAS`. For DSP-001-018 only, Jason Lin is authorized to use `STARSAAS` to create the dedicated branch, commits and Draft PR because the connected environment is authenticated only as `STARSAAS`; Robin Koh remains the authorized publishing maintainer. Package A's accurate Internal private location and future file scope are leadership-approved but excluded from public SWS; the public record retains only approval status, ownership, classification, opaque-reference status and safe implementation summary. Package B receives its Alias authority, control rules and isolated test environment; Package C selects DSP-003-004 as the future PORT-003 Safe Ledger Update input. These decisions close governance-design gaps only and do not start any Package, change permissions, create Package files, run `continue M001`, update the Ledger/freshness, activate policy or authorize SmartQuote Delivery. | Leadership-approved next-stage preparation; runtime remains Blocked; not a Package start authorization | SWS Pilot Packages A, B and C | DSP-001-018; one-time publishing exception expires on PR merge or Dispatch closure and creates no lasting role, permission or governance-model change |

## SWS-DEC-015 approved role matrices and boundaries

| Package | accountable_owner | maintainer | execution_owner | professional_reviewer | report_back_approver | Current status |
|---|---|---|---|---|---|---|
| Package A — SAIG | Robin Koh | Allen Liao | Allen Liao | Dorden | Jason Lin | Approved roles; Blocked pending remaining access, location and private-source conditions |
| Package B — M001 | Robin | Allen Liao | Allen Liao | Dorden | Jason Lin | Approved roles; Blocked pending Alias authority, files, fingerprints and execution authorization |
| Package C — Command Desk | Jason Lin | Allen Liao | Allen Liao | Dorden | Jason Lin | Approved roles; Blocked pending files, tool/permission verification, selected Report Back and safe-update evidence |

Approved overlap exception:

```yaml
overlap:
  person: Allen Liao
  roles:
    - maintainer
    - execution_owner
  reason: minimum SWS Pilot execution efficiency
  approved_by: Jason Lin
  scope: SWS Pilot Packages A, B and C only
  expiry: Pilot closure
  review_triggers:
    - Package completion
    - role change
    - access change
    - material finding
    - Pilot closure
  remaining_independent_reviewer: Dorden
```

Package C additionally permits Jason Lin to hold `accountable_owner` and `report_back_approver`; Dorden must still provide independent professional review. No overlap exception may remove all independent review.

Approved candidate locations and controls:

- Package A: existing private `STAR-SAAS/star-ai-governance`; Internal-only; no raw Confidential/Restricted data; Allen may prepare content but receives no automatic Write permission; submission uses an authorized maintainer's dedicated branch and PR. Exact private directory, actual access, authorized submitting maintainer, opaque public reference/private mapping, and retention/review implementation remain Missing.
- Package B: `docs/sws/PILOT_ALIAS_REGISTRY.md` and `docs/product-delivery/missions/M001/{CONTEXT_PACKAGE.md,ACTIVE_DECISIONS.md,WORK_STATUS.md` are Pilot Candidate paths only. `M001` must resolve uniquely; collisions stop and mark Blocked; chat or AI memory must not infer aliases. Alias owner, write authority and modification approval remain Missing. M1 and leadership commitment gates remain separate.
- Package C: `docs/sws/command-center/context/{CONTEXT_PACKAGE.md,ACTIVE_DECISIONS.md,WORK_STATUS.md` are Pilot Candidate paths. Ledger updates require a dedicated branch, one Portfolio Item, exact blob SHA or equivalent optimistic concurrency, complete PR diff, full post-write readback, structural/non-target checks, Dorden review and freshness change only after every check passes. Truncated-text reconstruction, unbound whole-file overwrite, forced SHA-conflict overwrite, unrelated multi-item updates and target-line-only verification are prohibited.

## SWS-DEC-016 identity, execution and package preparation record

### GitHub identity bindings

```yaml
github_identity_bindings:
  rkoh-star: Robin Koh
  STARSAAS: Jason Lin
  zhuangdongdong: Dorden
  liaoliesheng: Allen Liao
```

### Normal execution and publishing model

```yaml
execution_model:
  human_execution_owner: Allen Liao
  authorized_publishing_maintainer: Robin Koh
  publishing_github_account: rkoh-star
  independent_professional_reviewer: Dorden
  reviewer_github_account: zhuangdongdong
  report_back_approver: Jason Lin
```

Allen prepares content, execution instructions, verification and recovery handling. Robin performs authorized GitHub branch, commit and Draft PR publication. Dorden does not participate in primary preparation or writing and independently reviews the actual Exact Head. Jason Lin approves the final Report Back. Allen receives no repository permission increase; all file changes require a dedicated branch and PR.

### DSP-001-018 one-time publishing exception

```yaml
publishing_exception:
  scope: DSP-001-018 only
  authorized_publishing_maintainer: Robin Koh
  authorized_publishing_operator: Jason Lin
  publishing_github_account: STARSAAS
  human_execution_owner: Allen Liao
  independent_professional_reviewer: Dorden
  reviewer_github_account: zhuangdongdong
  report_back_approver: Jason Lin
  expiry: PR merge or DSP-001-018 closure
```

The exception permits Jason Lin / `STARSAAS` only to create the DSP-001-018 branch, commits and Draft PR. Robin Koh remains the authorized publishing maintainer. Dorden's independent review remains a mandatory Gate and cannot be replaced by Jason's publishing action. The exception creates no continuing role, permission or governance-model change and does not start any Package.

### Package A — approved next-stage preparation

```yaml
private_location_status:
  leadership_approved: true
  recorded_in_public_sws: false
  authoritative_private_record: Pending implementation in SAIG
classification: Internal
retention_owner: Robin Koh
review_owner: Dorden
public_reference_id: Pending runtime allocation
```

Package A's accurate Internal private location and future file scope are leadership-approved. Accurate location and file details may be recorded only in the private SAIG authoritative source. Public SWS retains only approval status, owners, classification, opaque-reference status and a safe implementation summary.

- future minimum necessary Read for `zhuangdongdong` is approved but not executed;
- a future private-source access test using purely synthetic data is approved but not executed;
- no Package A file is created and Wave A, Employee AI Use Policy and SAIG PILOT-001 remain inactive.

Public-record control from SWS-DEC-016 onward uses opaque references and safe summaries for private Package A sources. Earlier public historical records, including SWS-DEC-015 text, are not silently rewritten by this correction. Their classification remediation requires a separately authorized governance action.

### Package B — approved next-stage preparation

```yaml
alias_owner: Robin
human_execution_owner: Allen Liao
authorized_publishing_maintainer: Robin Koh
publishing_github_account: rkoh-star
modification_approver: Jason Lin
independent_reviewer: Dorden
```

Approved controls from DSP-003-004 include exact unique M001 resolution, collision detection with Blocked handling, migration, deprecation, tombstone, Pilot-exit retain/migrate/deprecate decisions, required-file fingerprinting, metadata-only refresh, partial reload, runtime-package reload, and stop/recovery rules.

Approved future isolated test environment:

```yaml
platform: ChatGPT Web
project: STAR OS
mode: Work
session_type: isolated controlled test session
professional_conversation: 🚀 Mission-001 · SmartQuote Foundation
test_prompt: continue M001
```

This approval does not create the Pilot Alias Registry or M001 Context Package, run `continue M001`, replace M1 or leadership commitment, mark M001 Committed or start SmartQuote Delivery.

### Package C — approved next-stage preparation

- future Safe Ledger Update target: `PORT-003`;
- selected verified professional input: `DSP-003-004 · Package B Remaining Missing Closure`;
- the formal `public_reference_id` must be randomly generated at execution time, opaque, and contain no person, project risk, Issue, URL or private path;
- the true mapping must remain outside the public Portfolio Ledger;
- no Portfolio Ledger or freshness update occurs under DSP-001-018;
- Package C Context Package remains uncreated and Package C remains Blocked.

## Not decided or frozen

- final SWS-001 v1.0 structure and freeze criteria;
- full Activity and Work Model;
- automated synchronization and generation of context packages;
- validated token and freshness thresholds by Scope and mode;
- final access model for sensitive portfolio information;
- exact final canonical location and naming convention for context packages in every repository;
- authoritative final Scope Alias Registry location and collision governance beyond the Pilot Candidate;
- whether future portfolio scale requires another management surface.
