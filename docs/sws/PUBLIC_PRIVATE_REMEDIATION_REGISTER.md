# SWS-001 · Public / Private Remediation Register

| Field | Value |
|---|---|
| Status | Pilot remediation record |
| Owner | STAR leadership |
| Maintainer | STAR Architecture maintainers |
| Last reviewed | 2026-07-21 |
| Classification | Public-safe metadata only |

This register records classification concerns without copying private paths, mappings, markers, credentials, employee details, customer facts or professional private evidence into the public repository.

| Historical record / decision | Classification concern | Current exposure | Sensitive data actually verified present | Required correction | Current disposition | Owner | Closure evidence | Blocks Draft PR #2 readiness |
|---|---|---|---|---|---|---|---|---|
| SWS-DEC-015 Package A preparation wording | Earlier wording did not consistently enforce opaque-reference and safe-summary boundaries for private authority details | Public governance text only | No verified disclosure of raw Confidential or Restricted data | Preserve history, add explicit current boundary and trace-review check; do not reproduce private details | Open for independent trace review | STAR Architecture maintainers | Final child PR exact diff and reviewer disposition | Yes, until reviewed |
| SWS-DEC-016 correction and later SWS records | Current model requires public approval status, ownership, classification and opaque status only | Public-safe summary model | No verified sensitive-data exposure | Verify all current records follow the corrected boundary | In progress | STAR Architecture maintainers | Consolidation checklist and trace review | Yes, until reviewed |
| Historical SWS Work Status Package detail | Current Work Status duplicated obsolete operational and professional detail | Public stale text; no private mapping retained in the consolidated version | No verified raw private data | Replace with concise current state and professional-source pointers | Corrected in DSP-001-044 child branch; pending review | STAR Architecture maintainers | `docs/sws/03_WORK_STATUS.md` final diff | No after review passes |
| Portfolio coordination records | Risk of importing professional detail into coordination status | Portfolio Ledger currently declares coordination-only boundary | No verified breach in current ledger review | Continue safe summaries and professional-source links only | Controlled / ongoing Pilot | STAR Command Desk | Portfolio Ledger operating rules and future readbacks | No |
| Scope Alias Registry | Alias mapping could expose private paths or be mistaken for professional truth | Minimal public-safe alias only | No | Allow verified public-safe source pointers; prohibit private mappings and status inference | Pilot | STAR Architecture maintainers | Alias Registry exact review and collision test | No, unless a finding appears |

## Disposition rules

- `Open for independent trace review` means classification treatment requires review; it does not mean a security incident occurred.
- `Corrected` means the current proposed record is changed but remains unverified until exact diff and final Head review.
- Unverified concern must not be described as confirmed leakage.
- Metadata correction does not imply compromise.
- A verified sensitive-data exposure would stop work and route to the appropriate private security, legal, compliance or AI Governance source.

## Closure criteria

1. Exact file list and diff reviewed.
2. No private path, mapping, marker, credential or sensitive professional detail present.
3. Historical decisions remain visible and are not silently rewritten.
4. Current records state the safe-summary and opaque-reference boundary.
5. Professional truth remains in owning professional sources.
6. Reviewer records Pass or Findings against the final Exact Head.

This register does not activate policy, resolve private professional evidence, pass a Gate, authorize product work, freeze or merge Draft PR #2.
