# [DEC-0034] Plan multi-step work before execution and report progress step by step

| Field | Value |
|---|---|
| **Type** | Governance / Working Method |
| **Status** | Accepted |
| **Owner** | STAR Product Delivery maintainers |
| **Decision date** | 2026-07-12 |
| **Effective date** | 2026-07-12 |
| **Review date / trigger** | Review if reporting becomes disruptive or fails to provide useful visibility |
| **Supersedes** | None |
| **Superseded by** | None |

## Context

STAR work may involve long research, documentation and GitHub update batches. Without concise progress reporting, the user cannot tell what is being completed, what remains, whether work is blocked or whether action is required.

## Decision

Before beginning a multi-step work batch, list the planned tasks in execution order. Then execute and report them step by step.

If no user or GitHub action is required, state that clearly and continue working. Progress reporting must remain concise and should not become a second long-form deliverable.

## Options considered

| Option | Benefits | Costs / risks | Why accepted or rejected |
|---|---|---|---|
| A. Report only at the end | Minimal interruption | Long periods of unclear status and hidden blockers | Rejected for material work batches |
| B. Announce every low-level operation | Maximum visibility | Noisy, distracting and hard to read | Rejected |
| C. List the batch first and provide milestone updates | Useful visibility with limited interruption | Requires discipline to keep updates concise | Accepted |
| D. Ask for confirmation before every step | Strong control | Slows reversible work and creates unnecessary decisions | Rejected except at defined decision gates |

## Rationale and evidence

- The user explicitly requested timely feedback and a planned, stepwise execution method.
- `DEC-0007` requires meaningful batches rather than stopping after every small item.
- `DEC-0008` limits escalation to material decisions.
- `DEC-0009` requires concise output.
- `DEC-0033` defines the minimum content of a progress update.

## Consequences

### Expected benefits

- The user can see current scope, progress, blockers and decision needs.
- Reversible work continues without unnecessary confirmation.
- GitHub work status and chat updates remain aligned.

### Trade-offs and risks accepted

- Excessive updates could create noise.
- Plans may change as evidence is discovered and must then be updated honestly.
- Progress reporting does not replace durable Markdown status.

### Required follow-up work

- Maintain `17_WORK_STATUS.md` for durable state.
- Use concise milestone updates during material batches.
- Record changed scope or blockers when they appear.

## Impact and relationships

- **Customers / users affected:** indirect; improves governance and delivery visibility.
- **Products / capabilities affected:** all STAR workstreams using this method.
- **Missions / work items affected:** multi-step research, architecture, documentation and implementation batches.
- **Teams / owners affected:** leadership, maintainers, AI collaborators and reviewers.
- **Related decisions and artifacts:** `DEC-0007`, `DEC-0008`, `DEC-0009`, `DEC-0033`, `07_WORKING_METHOD.md`, `17_WORK_STATUS.md`.

## Validation

- **Success evidence:** the user can identify planned work, current task, next action, blocker and required decision without reading operational detail.
- **Failure / revisit trigger:** reporting repeatedly interrupts work, omits blockers or fails to match the actual GitHub state.
- **Measurement owner:** STAR Product Delivery maintainers.
