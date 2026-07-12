# STAR Durable Knowledge Metadata

Use this header for material, reusable or decision-bearing Markdown. Do not add it to every temporary note.

```md
**Version:** v0.x.x  
**Status:** Candidate / Confirmed / Frozen / Superseded / Archived  
**Owner:** Accountable human or governance group  
**Maintainer:** Person, team or approved AI collaborator responsible for updates  
**Last reviewed:** YYYY-MM-DD  
**Review trigger:** Event that requires re-review  
**Authoritative source:** Repository path or external authoritative system  
**Scope:** Products, Missions, teams or decisions affected  
**Access classification:** Public / Internal / Confidential / Restricted
```

## Rules

1. **Owner is accountable; Maintainer performs upkeep.** They may be different.
2. **Status must describe authority, not writing progress.** A polished document can still be Candidate.
3. **Review trigger is required.** Prefer meaningful events over arbitrary dates when no review interval has been approved.
4. **Authoritative source must be unique.** Other copies are links or dated snapshots.
5. **Scope must be explicit.** Avoid allowing a local rule to appear enterprise-wide.
6. **Access classification follows the actual repository or source controls.** Do not place restricted information in a public repository.
7. **AI may maintain content only inside an authorized task and review boundary.** Human accountability remains explicit.

## Default review triggers for this baseline

Re-review when:

- a related confirmed decision is added, changed or superseded;
- a real Mission reveals a missing or unnecessary rule;
- the owner, maintainer, repository or authoritative source changes;
- a security, compliance, audit or incident finding affects the content;
- humans or AI receive contradictory guidance;
- the document is proposed for freeze, supersession or archival.
