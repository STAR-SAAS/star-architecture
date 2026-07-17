# SWS-001 · Work Status

| Field | Value |
|---|---|
| **Version / status** | v0.2.2 — Leadership startup conditions recorded; Packages not started |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Updated / last reviewed** | 2026-07-17 (Asia/Singapore) |
| **Authoritative working source** | Draft PR #2 working branch plus PR #5 child Draft PR record version until approved merge |
| **Scope** | SWS-001, conversation governance and SWS Pilot startup readiness |

## Current objective

Record the leadership-approved pre-start role matrices, candidate locations, overlap exception and safety boundaries for SWS Pilot Packages A, B and C without starting any Package or creating any Pilot file, while preserving the previously verified SWS-001 lifecycle and governance status.

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

## Leadership-approved startup conditions

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

Approved boundary:

- use existing private `STAR-SAAS/star-ai-governance`;
- classification is Internal-only;
- raw Confidential / Restricted data is prohibited;
- Allen Liao may prepare content but receives no automatic Write permission;
- actual submission must use an authorized maintainer's dedicated branch and PR;
- Dorden remains independent from primary execution;
- exact private directory, actual access, authorized submitting maintainer, opaque public reference/private mapping, retention/review implementation and private-source access test remain Missing.

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

Boundary:

- the Alias Registry path is Pilot Candidate only, not final canonical authority;
- `M001` must resolve uniquely to Mission-001;
- collisions stop and mark Blocked;
- chat history and AI memory cannot infer aliases;
- Alias owner, write authority and modification approval remain Missing;
- M1 and leadership commitment gates remain separate;
- no SmartQuote Delivery authorization is created.

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

Package C also permits Jason Lin to hold `accountable_owner` and `report_back_approver`; Dorden remains the required independent professional reviewer. No overlap exception removes independent review.

## Current state

| Area | State |
|---|---|
| Conversation Governance | Revised working baseline; not frozen |
| Decision history integrity | SWS-DEC-001 through SWS-DEC-015 preserved in canonical Decision Log; PR #5 review pending |
| Lifecycle / Contract model | Revised baseline preserved; operational validation pending |
| Sensitive-data controls | Revised generic structure; Package A Internal-only boundary approved; implementation Missing |
| File-level freshness | Revised design; runtime pilot Missing |
| Mode transfer | Candidate / environment-dependent |
| Scope Alias Registry | Pilot Candidate path approved; owner/write authority/approval Missing; file not created |
| `continue M001` | Not executed; conceptually validated / operationally Unverified |
| Package A roles | Confirmed by leadership; execution readiness Blocked |
| Package B roles | Confirmed by leadership; execution readiness Blocked |
| Package C roles | Confirmed by leadership; execution readiness Blocked |
| SAIG Context Package | Not created |
| Pilot Alias Registry | Not created |
| M001 Context Package | Not created |
| Command Desk Context Package | Not created |
| Command Center Portfolio Ledger | Stale / update pending; not modified by DSP-001-015 |
| Automatic context synchronization | Not authorized; inactive |
| Wave A / Employee AI Use Policy / SAIG PILOT-001 | Not activated |
| SmartQuote Delivery | Not started or authorized by this decision |
| Draft PR #2 | Open / Draft / unmerged; not frozen |

## Remaining Missing or required evidence

### Package A

1. Exact private directory path.
2. Allen Liao and related-role actual access verification.
3. Authorized submitting maintainer.
4. Opaque public reference and controlled private mapping.
5. Final retention and review implementation.
6. Private-source access test.

### Package B

1. Alias owner.
2. Write authority.
3. Alias modification approval workflow.
4. Context Package and Pilot Alias Registry files.
5. Required-file fingerprints.
6. Actual resume-test environment and execution authorization.

### Package C

1. Context Package files.
2. Actual execution tools and permission verification.
3. Write-time Ledger commit and blob SHA.
4. Exact professional Report Back selected for the end-to-end test.
5. Safe Ledger Update demonstration and independent-review evidence.

### Broader Candidate items

1. Numeric token and time-based freshness thresholds.
2. Direct mode-transfer capability by environment.
3. Manual versus generated/hybrid Context Package maintenance.
4. Whether a governed Reopened state is eventually needed.

## Next actions

1. Professionally review SWS-DEC-015 and the startup-readiness records in PR #5.
2. Confirm the role matrices and overlap exception were recorded without changing permissions or starting a Package.
3. Keep all three Packages Blocked until their Package-specific Remaining Missing items are resolved through separately authorized work.
4. Do not create Context Packages, the Pilot Alias Registry or update the Ledger without a later explicit Dispatch.

## Completion boundary

DSP-001-015 records leadership-approved startup conditions only. It does not start Package A, B or C; create any Context Package or Alias Registry; execute `continue M001`; update the Portfolio Ledger or freshness; change GitHub permissions; activate Wave A, Employee AI Use Policy or SAIG PILOT-001; mark M001 Committed; start SmartQuote Delivery; merge Draft PR #1 or #2; freeze SWS-001; or create, migrate or delete conversations.
