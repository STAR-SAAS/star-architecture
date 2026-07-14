# SWS-001 · STAR Command Center Minimum Launch Specification

| Field | Value |
|---|---|
| **Document ID** | SWS-CC-001 |
| **Version / status** | v0.1.0 — Confirmed working baseline; pilot not yet validated; not frozen |
| **Owner** | STAR leadership |
| **Maintainer** | STAR Architecture maintainers |
| **Last reviewed** | 2026-07-14 (Asia/Singapore) |
| **Decision references** | SWS-DEC-005 to SWS-DEC-009 |
| **Authoritative working source** | Draft PR #2, branch `agent/star-os-global-working-rules` |
| **Scope** | Minimum STAR Command Center pilot |

## 1. Purpose

STAR Command Center is the cross-project orchestration layer for STAR Workspace.

It answers:

- where new work enters;
- what has priority;
- where work should be routed;
- what the portfolio-level status is;
- what is blocked;
- what decision is needed;
- whether professional work has reported back;
- whether the portfolio ledger is current.

It does not replace the professional Projects, conversations, decision records, repositories or source systems where work is executed.

## 2. Minimum configuration

- Separate ChatGPT Project: `STAR Command Center`.
- Initial and only Chat: `⭐ STAR Command Desk`.
- No Weekly Planning, Monthly Review, Dashboard or other management conversations during the initial pilot.
- No migration, deletion or broad reorganization of existing conversations during the pilot.

## 3. Command Desk responsibilities

Command Desk is limited to:

1. intake;
2. clarification of work boundary;
3. prioritization;
4. routing;
5. portfolio-level status tracking;
6. blocker and dependency visibility;
7. decision-needed visibility;
8. receiving professional report-backs;
9. verifying available evidence;
10. updating the portfolio ledger;
11. concise feedback to the user.

## 4. Out of scope

Command Desk must not perform detailed:

- product design;
- architecture design;
- AI governance design;
- legal, compliance, finance or sales analysis;
- coding, testing or deployment;
- professional documentation belonging to another Scope;
- replacement of professional Decision Logs or Work Status records.

When work becomes professional, Command Desk routes it to the corresponding Project and conversation.

## 5. Authority boundary

`docs/sws/command-center/STAR-PORTFOLIO-STATUS.md` is authoritative for portfolio coordination status only:

- included workstreams;
- priority;
- routing destination;
- high-level state;
- current focus;
- next action;
- blocker;
- decision needed;
- authoritative professional-source link;
- last reported and last verified dates;
- freshness.

It is not authoritative for detailed architecture, governance, product requirements, code, test evidence, customer data, employee data, risk registers or live tool entitlements.

Detailed truth remains in the linked professional source.

## 6. Operating loop

```text
Dispatch → Execute → Report Back → Verify → Update Status → Feedback
```

### Dispatch

Command Desk identifies the Scope, destination Project and conversation, objective, expected output, applicable decisions, sources, constraints and required report-back.

Minimum dispatch fields:

```text
Dispatch ID:
Portfolio Item:
Destination Project:
Destination Conversation:
Objective:
Current Scope:
Expected Output:
Applicable Confirmed Decisions:
Authoritative Sources:
Known Constraints:
Open Questions:
Required Report Back:
```

### Execute

Professional work occurs in the destination Project and conversation. That space owns professional analysis, decisions, artifacts, GitHub action, validation and specialist status.

### Report Back

Minimum report-back fields:

```text
Portfolio Item:
Professional Scope:
Status:
Completed:
Current Result:
Authoritative Record:
Next Action:
Blocker:
Decision Needed:
Last Verified At:
```

### Verify

A report is not automatically verified because it appeared in chat. Command Desk checks the authoritative source where available or marks the state Unknown / unverified.

### Update Status and Feedback

Command Desk updates the portfolio ledger after each material verified change, then provides concise portfolio-level feedback or redispatches the work.

## 7. Portfolio model

### Status values

- Intake
- Routed
- Active
- Waiting
- Blocked
- Review
- Closed

### Priority values

- Now
- Next
- Later
- Parked

### Freshness values

- Current
- Stale
- Unknown

Do not use unverified percentages or vague states such as “almost done.”

## 8. Minimum portfolio fields

Each item records:

- Item ID;
- Title;
- Workstream;
- Item Type;
- Priority;
- Status;
- Professional Project;
- Professional Conversation;
- Accountable Owner;
- Current Focus;
- Next Action;
- Blocker;
- Decision Needed;
- Authoritative Source;
- Last Reported At;
- Last Verified At;
- Freshness.

Missing data remains explicitly Missing or Unknown.

## 9. Pilot scope

The pilot includes only:

1. SWS-001 · STAR Workspace Specification;
2. STAR AI Governance;
3. Mission-001 · SmartQuote Foundation.

These test platform architecture, governance and product/Mission coordination without expanding the system prematurely.

## 10. Pilot start conditions

- STAR Command Center Project exists.
- `⭐ STAR Command Desk` exists.
- Project Instructions are installed and verified.
- The authoritative portfolio ledger exists.
- The initial three Portfolio Items exist.
- Each item identifies its professional Project and conversation.
- Each item links a verified professional authoritative source.
- Initial status is verified rather than inferred.
- Dispatch and Report Back formats are available.
- No existing conversation has been moved or deleted.

## 11. Pilot evidence required

The pilot should demonstrate:

- one correctly routed new item;
- one material SWS report-back;
- one SAIG status update without sensitive-detail duplication;
- one SmartQuote Mission status update;
- one correctly surfaced blocker;
- one precise leadership decision request;
- one honest Stale or Unknown state;
- one item closed with evidence;
- no professional execution accidentally performed in Command Desk;
- no status based only on chat memory.

## 12. Expansion and migration

Additional management surfaces require observed evidence such as sustained Command Desk overload, recurring planning needs, access separation or Markdown readability failure.

Any migration requires a separately reviewed plan containing current location, target location, authority impact, links, retention, owner, validation and rollback.

## 13. Launch readiness

The architecture is ready for a controlled minimum pilot, but the pilot is not active until:

- Project Instructions are verified;
- all three initial items are populated from authoritative sources;
- the first update loop is successfully evidenced.

This specification does not declare SWS-001 complete, approved or frozen.
