# Changelog

All notable changes to this Markdown baseline are recorded here.

## [0.1.7] — 2026-07-12

### Added

- `16_ACTIVE_MISSION_INTAKE.md` with the current evidence-gap audit for Mission-001 and Mission-002.
- `17_WORK_STATUS.md` with current tasks, progress, blockers, next actions and user-decision status.

### Verified

- `STARSAAS/star-platform` and `STARSAAS/star-domains` currently contain no repository material that can serve as an authoritative real-Mission baseline.
- The SmartQuote discount-rule and GateHub PSP-connector files remain desk examples, not completed real-Mission validation.

### Corrected

- Aligned README and Manifest with the actual Draft PR file set.
- Added the active-Mission intake and work-status files to the repository reading order and index.
- Clarified that no user GitHub action is currently required and Draft PR #1 should not yet be merged.

## [0.1.6] — 2026-07-12

### Added

- Recorded `DEC-0033`: STAR work must include timely, concise progress feedback while tasks are underway.

### Improved

- Progress feedback now has an explicit minimum shape: current task, purpose, status, next action, blocker if any, and whether a user decision is needed.

## [0.1.5] — 2026-07-12

### Added

- `13_INFORMATION_AND_KNOWLEDGE_GOVERNANCE.md` with a candidate authoritative-source map and knowledge lifecycle.
- `14_AI_WORK_GOVERNANCE.md` with candidate AI work levels, human accountability and stop conditions.
- `15_VALIDATION_PLAN.md` defining the evidence required before freeze.
- `templates/DECISION_RECORD.md` as a generic cross-domain Decision Record candidate.
- Two concise Mission Brief examples for SmartQuote discount rules and a GateHub PSP connector.

### Improved

- Added role-based reading guidance so front-line teams do not need to read the research repository.
- Made the Mission Brief the primary team-facing artifact while keeping detailed evidence linked.
- Replaced abstract open questions with concrete candidate artifacts and validation actions.
- Kept the foundation in Draft status; no candidate rule was promoted to a confirmed or frozen standard.

## [0.1.3] — 2026-07-12

### Added

- One-page `11_FOUNDATION_CANDIDATE.md` with the minimum delivery loop, Mission definition, entry/exit boundaries and minimum information objects.
- `12_RESPONSIBILITY_AND_ROLE_VIEWS.md` to separate value receiver, stakeholder, owner, approver, reviewer, operator, AI agent and system responsibilities.
- `templates/MISSION_BRIEF.md` as the first team-facing template for real-Mission validation.

### Changed

- Made the one-page foundation and Mission Brief the primary README entry points.
- Linked open questions and assumptions to concrete validation artifacts instead of leaving them as abstract research topics.
- Replaced the stale manually maintained SHA-256 table with Git-based integrity guidance and a live file index.

### Still open

- The candidate model is not frozen until it is used on a real active Mission with actual owners, dates, dependencies, approvals and outcome evidence.
- Final STAR scope/name, Mission hierarchy, AI authority boundaries and authoritative-source mapping remain open.

## [0.1.2] — 2026-07-12

### Changed

- Confirmed `STARSAAS/star-architecture` as the repository for this baseline.
- Set the target path to `docs/product-delivery/`.
- Published the baseline on branch `agent/star-os-product-delivery-baseline` and opened Draft PR #1.
- Clarified that GitHub storage does not freeze or approve the working baseline.
- Recorded repository/path confirmation as `DEC-0032` and resolved `OQ-006` / `ASM-008`.

## [0.1.1] — 2026-07-12

### Added

- Initial delivery-model validation using a SmartQuote merchant discount rule and a GateHub PSP connector.
- Candidate minimum information model and role-specific Mission view.

### Learned

- Need/value → Mission → work → release → learning is a useful backbone, but ownership, decision, risk/approval, traceability and current state must cross the full lifecycle.
- Team-facing views should start with why, what, who, now and evidence; deep architecture and research should be drill-down content.

## [0.1.0] — 2026-07-12

### Added

- Project Charter
- Consolidated Decision Log with 31 working decisions
- Open Questions register
- Source-reviewed Research Canon candidate
- Superseded and rejected ideas register
- Assumptions register
- Cross-functional Stakeholder Map
- Working Method and quality checks
- Audit of the three early Product Delivery drafts
- Working Glossary
- Explicit GitHub synchronization status

### Corrected

- Reclassified early documents labelled v1.0 as draft v0.1 concepts pending proper validation.
- Replaced premature "fully adopt" language with contextual minimum-adoption candidates.
- Separated confirmed decisions from hypotheses and open questions.

### Known limitations at this version

- GitHub repository destination had not yet been confirmed.
- Files had not yet been pushed to GitHub.
- Several previously discussed frameworks still required primary-source audit.
- Final STAR scope, Mission definition and minimal meta-model remained open.
