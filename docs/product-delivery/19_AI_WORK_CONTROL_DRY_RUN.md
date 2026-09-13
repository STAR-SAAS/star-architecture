# STAR AI Work-Control Dry Run — GitHub Documentation Batch

**Version:** v0.1.0  
**Status:** Validation evidence; AI governance remains candidate  
**Purpose:** Test the A2 reversible-execution controls in `14_AI_WORK_GOVERNANCE.md` against actual GitHub documentation work.

## Task under test

Create and update the Product Delivery Markdown baseline in `STARSAAS/star-architecture` on branch `agent/star-os-product-delivery-baseline`, keep Draft PR #1 accurate, and avoid changing `main` or claiming that candidate content is frozen.

## Work-level classification

- **A1 — Propose:** draft and revise Markdown content, models, templates and validation findings.
- **A2 — Execute reversible:** create/update files on a dedicated branch and update the Draft PR description.
- **Not authorized:** merge the PR, write directly to `main`, approve/freeze standards, expose secrets, delete repositories or perform production/customer actions.

## Authorization evidence

- The user explicitly approved `STARSAAS/star-architecture/docs/product-delivery/` as the destination.
- The user instructed the work to continue when no decision was required.
- `DEC-0032` requires branch/PR review rather than direct changes to `main`.
- `DEC-0033` and `DEC-0034` require timely and stepwise progress reporting.

## Minimum control record

| Control | Applied evidence |
|---|---|
| **Task** | Build and maintain the reviewable Product Delivery Markdown baseline |
| **Scope** | `STARSAAS/star-architecture`, Product Delivery directory, dedicated branch and Draft PR #1 |
| **Context** | Decision Log, Open Questions, Working Method, existing branch files and current PR state |
| **Allowed actions** | Create/update UTF-8 Markdown on the branch; update Draft PR description; read repository/PR state |
| **Prohibited actions** | Merge, write to `main`, freeze candidate content, change unrelated repositories, expose secrets or perform high-impact operations |
| **Risk level** | A2 — reversible repository changes on a review branch |
| **Human accountability** | STAR leadership/user retains acceptance, freeze and merge authority |
| **Traceability** | Git commits, file history, Draft PR #1, Decision Log, Changelog and Work Status |
| **Expiry / stop trigger** | Scope changes materially, conflicting confirmed decision appears, user directs stop, or merge/high-impact action is requested |

## Controls observed

- Changes were made on a dedicated branch rather than `main`.
- The PR remained Draft and unmerged.
- Candidate, confirmed and frozen states remained separate.
- Repository and PR state were re-read before claims were made.
- A stale manual checksum mechanism was removed rather than presented as reliable.
- Missing Mission data was recorded as a blocker instead of being invented.
- The user was told when no GitHub action was required.
- A write conflict on `15_VALIDATION_PLAN.md` caused the current file to be re-read before retrying; the file was not overwritten using stale state.

## Outcome

The A2 control model worked for this bounded documentation and GitHub task:

- all changes remain reviewable and reversible;
- no main-branch or production action occurred;
- human acceptance and merge authority were preserved;
- evidence exists through commits and the Draft PR;
- uncertainty and blockers were recorded explicitly.

## Gaps found

- Authorization expiry should be stated per work batch, not assumed indefinitely.
- A2 execution still needs repository/path/action boundaries stated clearly when more than one repository is involved.
- Review quality is not proven merely because a change is on a branch; accountable content review is still required.
- This test does not validate AI-generated code, test execution, sensitive data use or production operations.

## V5 result

**Status:** Partial.

**Validated:** A1 document proposal and A2 reversible GitHub execution.

**Still required:**

- one AI code or test proposal with automated and human review evidence;
- one bounded sandbox/tool execution outside documentation;
- one A3 high-impact scenario as a dry run only, including approval, rollback and escalation boundaries.
