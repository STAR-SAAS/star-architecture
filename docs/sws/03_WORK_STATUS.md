# SWS-001 · Work Status

| Field | Value |
|---|---|
| **Version / status** | v0.2.3 — Leadership next-stage preparation decisions recorded; Packages not started |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Updated / last reviewed** | 2026-07-17 (Asia/Singapore) |
| **Authoritative working source** | Draft PR #2 working branch plus DSP-001-018 child Draft PR record version until approved merge |
| **Scope** | SWS-001, conversation governance and SWS Pilot startup readiness |

## Current objective

Record the leadership-approved identity bindings, execution/publishing/review model, DSP-001-018 one-time publishing exception and Package A/B/C next-stage preparation decisions without starting any Package, creating Package files, changing permissions, executing tests or updating the Portfolio Ledger, while enforcing the public/private boundary for Package A through opaque references and safe summaries.

## Verified completed revision work

- Restored the original SWS-DEC-006 wording, including `STARSAAS/star-architecture`.
- Added SWS-DEC-014 for the later transfer to `STAR-SAAS/star-architecture` without erasing historical wording.
- Distinguished leadership-confirmed decision basis, child Draft PR proposed record version and authority after merge into Draft PR #2.
- Replaced the linear lifecycle with a primary path plus Waiting / Blocked interrupt states and recorded recovery behavior.
- Clarified transfer, closure and Contract reuse rules.
- Added executable Context Package classification, audience, redaction, private-source, evidence-access and retention/review metadata.
- Preserved SAIG authority for AI privacy, retention, employee-data, audit and AI-record controls.
- Added required-file blob/version verification and metadata-only no-reload behavior.
- Marked direct mode switching and seamless context inheritance Candidate / environment-dependent.
- Added Closed / Superseded Questions provenance, including SWS-OQ-003.
- Added SWS-OQ-014 for the authoritative Scope Alias Registry.
- Kept `continue M001` as conceptually validated / operationally Unverified.
- Recorded SWS-DEC-015 role matrices, overlap exception and Package A/B/C startup boundaries.
- Recorded SWS-DEC-016 identity bindings, unified execution model, next-stage preparation decisions and the temporary DSP-001-018 publishing exception.
- Corrected the DSP-001-018 Package A public/private boundary so public SWS records retain only opaque-reference status and safe summaries, while accurate private location and file details remain in the private authority.

## Revised lifecycle model

Primary path:

```text
Intake → Routed → Bootstrapped → Active → Review → Closed
```

Interrupt behavior:

- Waiting and Blocked may be entered from Routed, Bootstrapped, Active or Review.
- `prior_state` is recorded before interruption.
- Waiting returns to `prior_state` when awaited input arrives.
- Blocked returns to `prior_state` after blocker resolution.
- Transfer starts the receiver at Bootstrapped and ends the sender's active ownership.
- Closed is not silently reopened; new work uses a new Activity / Contract unless a governed Reopened rule is approved.

## Leadership-approved identity and execution model

### GitHub identity bindings

```yaml
github_identity_bindings:
  rkoh-star: Robin Koh
  STARSAAS: Jason Lin
  zhuangdongdong: Dorden
  liaoliesheng: Allen Liao
```

### Normal execution model

```yaml
execution_model:
  human_execution_owner: Allen Liao
  authorized_publishing_maintainer: Robin Koh
  publishing_github_account: rkoh-star
  independent_professional_reviewer: Dorden
  reviewer_github_account: zhuangdongdong
  report_back_approver: Jason Lin
```

Execution boundary:

- Allen prepares content, execution instructions, verification and recovery handling;
- Robin performs authorized GitHub branch, commit and Draft PR publication;
- Dorden does not participate in primary preparation or writing and independently reviews the actual Exact Head;
- Jason Lin approves the final Report Back;
- Allen receives no repository permission increase;
- all file changes require a dedicated branch and PR.

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

The exception permits Jason Lin / `STARSAAS` only to create the DSP-001-018 branch, commits and Draft PR because the connected environment is authenticated as `STARSAAS`. Robin Koh remains the authorized publishing maintainer. Dorden's independent review remains mandatory and cannot be replaced by Jason's publishing action. The exception creates no continuing role, permission or governance-model change and does not start any Package.

## Leadership-approved startup and next-stage preparation conditions

### Package A — SAIG

```yaml
accountable_owner: Robin Koh
maintainer: Allen Liao
execution_owner: Allen Liao
professional_reviewer: Dorden
report_back_approver: Jason Lin
owner_status: Confirmed
current_status: Blocked
```

Public-safe approved boundary and preparation record:

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

- Package A's accurate Internal private location and future file scope are leadership-approved but may be recorded only in the private SAIG authoritative source;
- public SWS records only approval status, owners, classification, opaque-reference status and a safe implementation summary;
- raw Confidential / Restricted data remains prohibited from the public SWS record;
- Allen Liao may prepare content but receives no automatic Write permission;
- actual publication follows the authorized publishing model and uses a dedicated branch and PR;
- future minimum necessary Read for `zhuangdongdong` is approved but not granted;
- future private-source access test is approved only with purely synthetic data and has not run;
- Dorden remains independent from primary execution;
- Wave A, Employee AI Use Policy and SAIG PILOT-001 remain inactive.

Remaining Missing:

1. `zhuangdongdong` Read has not been granted or verified.
2. Private-source access test has not been executed.
3. Package files have not been created.
4. Private authoritative record remains Pending implementation in SAIG.
5. Runtime `public_reference_id` has not been allocated.

Public-record control from SWS-DEC-016 onward uses opaque references and safe summaries for private Package A sources. Earlier public historical records, including SWS-DEC-015 text, are not silently rewritten by this correction. Their classification remediation requires a separately authorized governance action.

### Package B — M001

```yaml
accountable_owner: Robin
maintainer: Allen Liao
execution_owner: Allen Liao
professional_reviewer: Dorden
report_back_approver: Jason Lin
owner_status: Confirmed
current_status: Blocked
```

Approved Pilot Candidate paths:

```text
docs/sws/PILOT_ALIAS_REGISTRY.md
docs/product-delivery/missions/M001/CONTEXT_PACKAGE.md
docs/product-delivery/missions/M001/ACTIVE_DECISIONS.md
docs/product-delivery/missions/M001/WORK_STATUS.md
```

Approved authority:

```yaml
alias_owner: Robin
human_execution_owner: Allen Liao
authorized_publishing_maintainer: Robin Koh
publishing_github_account: rkoh-star
modification_approver: Jason Lin
independent_reviewer: Dorden
```

Approved controls:

- `M001` must resolve exactly and uniquely to Mission-001;
- collisions stop execution and mark Blocked;
- chat history and AI memory cannot infer aliases;
- migration, deprecation and tombstone behavior is governed;
- Pilot exit requires an explicit retain / migrate / deprecate decision;
- required-file fingerprints govern runtime integrity;
- metadata-only refresh, partial reload and runtime-package reload are supported under the approved rules;
- stop and recovery rules from DSP-003-004 apply;
- M1 and leadership commitment gates remain separate;
- no SmartQuote Delivery authorization is created.

Approved future isolated test environment:

```yaml
platform: ChatGPT Web
project: STAR OS
mode: Work
session_type: isolated controlled test session
professional_conversation: 🚀 Mission-001 · SmartQuote Foundation
test_prompt: continue M001
```

Remaining Missing:

1. Package files and Pilot Alias Registry have not been created.
2. Required-file fingerprints have not been generated.
3. Access capability has not been executed or verified.
4. `continue M001` has not been run.
5. M1 has not passed.
6. Leadership commitment has not passed.
7. M001 is not Committed and SmartQuote Delivery is not started or authorized.

### Package C — Command Desk

```yaml
accountable_owner: Jason Lin
maintainer: Allen Liao
execution_owner: Allen Liao
professional_reviewer: Dorden
report_back_approver: Jason Lin
owner_status: Confirmed
current_status: Blocked
```

Approved Pilot Candidate paths:

```text
docs/sws/command-center/context/CONTEXT_PACKAGE.md
docs/sws/command-center/context/ACTIVE_DECISIONS.md
docs/sws/command-center/context/WORK_STATUS.md
```

Approved future Safe Ledger Update input:

```yaml
target_portfolio_item: PORT-003
professional_input: DSP-003-004 · Package B Remaining Missing Closure
public_reference_id:
  generation: random at formal execution time
  required_property: opaque
  prohibited_content:
    - person
    - project risk
    - Issue
    - URL
    - private path
  true_mapping_location: outside the public Portfolio Ledger
```

Approved Safe Ledger Update sequence:

```text
dedicated branch
→ one Portfolio Item minimal change
→ exact blob SHA or equivalent optimistic concurrency
→ complete PR diff
→ full post-write readback
→ verify file boundaries, structure, Item count and non-target regions
→ Dorden independent review
→ freshness update only after every validation passes
```

Prohibited paths include truncated-text reconstruction, whole-file replacement without SHA binding, forced overwrite after SHA conflict, unrelated multi-item updates and target-line-only post-write verification.

Remaining Missing:

1. Package C files have not been created.
2. Formal `public_reference_id` has not been generated.
3. Write-time authoritative branch Head and Ledger blob SHA have not been obtained.
4. Safe Ledger Update has not been executed.
5. Portfolio Ledger and freshness remain unmodified.
6. Dorden has not independently reviewed the actual Ledger PR Exact Head.

## Approved role-overlap exception

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

Package C also permits Jason Lin to hold `accountable_owner` and `report_back_approver`; Dorden remains the required independent professional reviewer. No overlap or publishing exception removes independent review.

## Current state

| Area | State |
|---|---|
| Conversation Governance | Revised working baseline; not frozen |
| Decision history integrity | SWS-DEC-001 through SWS-DEC-016 preserved in canonical Decision Log; DSP-001-018 Draft PR review pending |
| Lifecycle / Contract model | Revised baseline preserved; operational validation pending |
| Identity bindings | Confirmed by leadership; operational use remains task-scoped |
| Normal publishing model | Robin Koh / `rkoh-star`; not changed by DSP-001-018 exception |
| DSP-001-018 publishing exception | Confirmed; valid until PR merge or Dispatch closure |
| Package A public/private boundary | Corrected for SWS-DEC-016 onward: public record uses opaque references and safe summaries; historical remediation remains separate |
| Sensitive-data controls | Package A Internal boundary approved; implementation Missing |
| File-level freshness | Revised design; runtime pilot Missing |
| Mode transfer | Candidate / environment-dependent |
| Scope Alias Registry | Pilot Candidate path and authority approved; file not created |
| `continue M001` | Not executed; governance controls and test environment approved; operationally Unverified |
| Package A | owner_status Confirmed; current_status Blocked |
| Package B | owner_status Confirmed; current_status Blocked |
| Package C | owner_status Confirmed; current_status Blocked |
| SAIG Context Package | Not created |
| Pilot Alias Registry | Not created |
| M001 Context Package | Not created |
| Command Desk Context Package | Not created |
| Command Center Portfolio Ledger | Stale / update pending; not modified by DSP-001-018 |
| Automatic context synchronization | Not authorized; inactive |
| Wave A / Employee AI Use Policy / SAIG PILOT-001 | Not activated |
| SmartQuote Delivery | Not started or authorized |
| Draft PR #2 | Open / Draft / unmerged; not frozen |

## Next actions

1. Return the corrected PR #6 Exact Head to Command Desk for public/private boundary verification.
2. Obtain Dorden's independent review only against the corrected actual Exact Head through `zhuangdongdong` after access is available.
3. Keep the Draft PR unmerged until Command Desk verifies the Report Back and separately authorizes merge.
4. Keep all three Packages Blocked until their Package-specific Remaining Missing items are closed through separately authorized work.
5. Do not grant access, create Package files or Registry, run `continue M001`, update the Ledger/freshness or start any Package under DSP-001-018.

## Completion boundary

DSP-001-018 records leadership-approved identity bindings, execution/publishing/review responsibilities, one temporary publishing exception and next-stage preparation decisions only. It does not start Package A, B or C; change GitHub permissions; grant `zhuangdongdong` Read; create any Context Package or Pilot Alias Registry; execute `continue M001`; generate runtime fingerprints or public references; update the Portfolio Ledger or freshness; activate Wave A, Employee AI Use Policy or SAIG PILOT-001; mark M001 Committed; start SmartQuote Delivery; merge Draft PR #1 or #2; or freeze SWS-001.
