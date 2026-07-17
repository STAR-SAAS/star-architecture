# SWS-001 · Open Questions and Missing Evidence

| Field | Value |
|---|---|
| **Version / status** | v0.2.3 — Active |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-17 (Asia/Singapore) |
| **Authoritative working source** | Draft PR #2 working branch plus DSP-001-018 child Draft PR record version until approved merge |
| **Scope** | SWS-001, STAR Command Center pilot and conversation-governance pilot |

Open questions and missing evidence must not be presented as confirmed architecture or verified operational state. Prior Question IDs remain visible when closed, superseded or reformulated.

## Priority A — required pilot evidence

| ID | Question or missing evidence | State | Required next evidence |
|---|---|---|---|
| **SWS-OQ-001** | Are final STAR Command Center Project Instructions installed closely enough to enforce orchestration-only behavior? | Missing | Compare installed Project Instructions with SWS-CC-001. |
| **SWS-OQ-002** | What is the verified current professional status and owner of each pilot workstream? | Leadership-approved role, identity and publishing models recorded; runtime evidence still incomplete | Verify Package-specific access, files, test execution and independent-review evidence against SWS-DEC-015 and SWS-DEC-016. |
| **SWS-OQ-004** | Can Command Desk maintain the portfolio ledger reliably? | Safe-update method and PORT-003 input approved; execution Missing; portfolio ledger remains Stale / unmodified | Execute the approved Safe Ledger Update on PORT-003 using DSP-003-004, a runtime-generated opaque reference, exact commit/blob, full readback, diff, recovery point and Dorden review evidence. |
| **SWS-OQ-010** | Where will each pilot Scope place its canonical Context Package, Active Decisions and Work Status? | Package A private location and future file scope leadership-approved but excluded from public SWS; Package B and C Pilot Candidate paths approved; files not created | Record Package A implementation details only in the private SAIG authority; create and review Package files only under later explicit authorization. |
| **SWS-OQ-011** | Can `continue M001` resolve the correct Scope, conversation, branch and runtime package without user reconstruction? | Governance controls and isolated test environment approved; operationally Unverified | Create approved files and fingerprints in later authorized work, verify access capability, then run the isolated controlled `continue M001` test. |
| **SWS-OQ-014** | Where is the authoritative Scope Alias Registry? | Pilot Candidate path and Alias authority approved; Registry not created | Create `docs/sws/PILOT_ALIAS_REGISTRY.md` only under later explicit authorization, then verify owner, publishing, modification approval and collision controls. |
| **SWS-OQ-015** | Are classification, audience, redaction and evidence-access fields sufficient across public and private Context Packages? | Package A Internal classification and ownership approved; private location excluded from public SWS; implementation Unverified | Grant and verify minimum Read for `zhuangdongdong`, implement the private authoritative record when authorized, and run the synthetic-data private-source access test. |

## Package-specific Remaining Missing under SWS-DEC-016

### Package A — SAIG

Confirmed preparation decisions safe for the public SWS record:

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

- The accurate Internal private location and future file scope are leadership-approved but may appear only in the private SAIG authoritative source.
- Future minimum necessary Read for `zhuangdongdong` is approved.
- Future private-source access testing is restricted to purely synthetic data.

Remaining Missing:

- `zhuangdongdong` Read has not been granted or verified;
- private-source access test has not been executed;
- Package files have not been created;
- private authoritative record remains Pending implementation in SAIG;
- runtime `public_reference_id` has not been allocated;
- no Wave A, Employee AI Use Policy or SAIG PILOT-001 activation has occurred.

Public-record control from SWS-DEC-016 onward requires opaque references and safe summaries. Earlier public historical classification issues require a separately authorized governance action and are not silently rewritten here.

### Package B — M001

Confirmed preparation decisions:

- Alias owner: Robin;
- human execution owner: Allen Liao;
- authorized publishing maintainer: Robin Koh through `rkoh-star`;
- modification approver: Jason Lin;
- independent reviewer: Dorden;
- exact unique M001 resolution, collision/Blocked handling, migration, deprecation, tombstone and Pilot-exit controls approved;
- required-file fingerprint, metadata-only refresh, partial reload, runtime-package reload and stop/recovery rules approved;
- isolated future test environment approved: ChatGPT Web / STAR OS / Work / isolated controlled test session / `🚀 Mission-001 · SmartQuote Foundation` / `continue M001`.

Remaining Missing:

- Package files and Pilot Alias Registry have not been created;
- required-file fingerprints have not been generated;
- access capability has not been executed or verified;
- `continue M001` has not been run;
- M1 has not passed;
- leadership commitment has not passed;
- M001 is not Committed and SmartQuote Delivery is not authorized.

### Package C — Command Desk

Confirmed preparation decisions:

- future target Portfolio Item: `PORT-003`;
- selected professional input: `DSP-003-004 · Package B Remaining Missing Closure`;
- runtime `public_reference_id` must be random, opaque and exclude persons, project risks, Issues, URLs and private paths;
- the true mapping must remain outside the public Portfolio Ledger;
- Safe Ledger Update controls from SWS-DEC-015 remain mandatory.

Remaining Missing:

- Package C files have not been created;
- formal `public_reference_id` has not been generated;
- write-time authoritative branch Head and Ledger blob SHA have not been obtained;
- Safe Ledger Update has not been executed;
- Portfolio Ledger and freshness remain unmodified;
- Dorden has not independently reviewed the actual Ledger PR Exact Head.

## Priority B — usability and efficiency validation

| ID | Question or missing evidence | Validation approach |
|---|---|---|
| **SWS-OQ-005** | Does the Dispatch package provide enough context without duplicating professional history? | Compare real dispatches across SWS, SAIG and M001. |
| **SWS-OQ-006** | Is Report Back concise and complete enough to update durable status? | Compare actual report-backs and ledger updates. |
| **SWS-OQ-007** | What makes a Scope Current, Stale or Unverified? | Test file-level fingerprints and observe operational cadence before fixing time thresholds. |
| **SWS-OQ-008** | Does one Command Desk remain sufficient? | Record actual overload, routing failure or access conflict. |
| **SWS-OQ-009** | Is the public architecture repository appropriate for each coordination record? | Classify real entries; retain sensitive detail in private sources. |
| **SWS-OQ-012** | What token/file budgets are safe and useful for Chat, Work and Codex? | Measure entrypoint, required payload, optional and evidence loads during pilots. |
| **SWS-OQ-013** | Should Context Packages be manually maintained, generated or hybrid? | Pilot manual packages before proposing automation. |
| **SWS-OQ-016** | Which environments support direct mode transfer and seamless Contract/context inheritance? | Record actual platform behavior; use Handoff when unavailable. |
| **SWS-OQ-017** | Should Closed work ever use a governed Reopened state? | Observe pilot needs; until decided, use a new Activity / Contract. |

## Closed / Superseded Questions

| ID | Closure status | Closure basis | Evidence | Closure date | Replacement question |
|---|---|---|---|---|---|
| **SWS-OQ-003** | Closed for minimum pilot; ownership detail remains source-specific | Named ownership is required by the Contract and Context Package; absent owners remain Missing rather than blocking the generic model | SWS-DEC-010 and Contract/Context Package fields in PR #3 | 2026-07-17 | SWS-OQ-002 continues verification of actual pilot owners |

No other prior Question ID is closed or deleted by this revision.

## Confirmed matters not to reopen without new evidence

- Correct Project and professional conversation are stated proactively.
- Brief warnings are used for mode mismatch.
- Users are not asked to repeat decisions available in authoritative records.
- GitHub stores durable structured memory, not raw chat archives.
- Runtime loading is progressive and file-level incremental; whole-repository and full-history loading are not default.
- No existing conversations are migrated or deleted by this baseline.
- The baseline is not frozen.
- SAIG retains authority for AI privacy, retention, employee-data, audit and AI-record controls.
- SWS-DEC-015 approves startup conditions only; it does not start a Package or create its files.
- SWS-DEC-016 closes named governance-design gaps only; it does not execute access, file creation, tests, Ledger updates or Package starts.
- Public SWS records use opaque references and safe summaries for private Package A sources; accurate private locations and mappings remain outside this public repository.
- The DSP-001-018 publishing exception is temporary, scoped only to that Dispatch and expires on PR merge or Dispatch closure.

## Deferred broader work

- complete Activity and Work Model;
- automatic Context Package generation and synchronization;
- future Agent orchestration;
- final role-specific Workspace views;
- full Memory and Knowledge lifecycle beyond the current structured-memory baseline.
