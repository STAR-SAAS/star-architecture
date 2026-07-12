# [DEC-0032] Store the Product Delivery baseline in the STAR architecture repository

| Field | Value |
|---|---|
| **Type** | Architecture / Repository Governance |
| **Status** | Accepted |
| **Owner** | STAR architecture and Product Delivery maintainers |
| **Decision date** | 2026-07-12 |
| **Effective date** | 2026-07-12 |
| **Review date / trigger** | Review when repository boundaries or ownership materially change |
| **Supersedes** | None |
| **Superseded by** | None |

## Context

Confirmed Product Delivery knowledge needed a durable and reviewable location. The available repositories were `star-architecture`, `star-platform` and `star-domains`. The baseline contains cross-cutting product-delivery, architecture and governance material rather than application code or domain implementation.

## Decision

Store the Product Delivery working-memory baseline in `STARSAAS/star-architecture` under `docs/product-delivery/`.

Introduce and review the baseline through a dedicated branch and Draft pull request rather than writing it directly to `main`.

## Options considered

| Option | Benefits | Costs / risks | Why accepted or rejected |
|---|---|---|---|
| A. Store in `star-architecture/docs/product-delivery/` | Fits cross-cutting architecture/engineering knowledge; versioned and reviewable | Repository scope may need later refinement | Accepted |
| B. Store in `star-platform` | Could place all STAR platform material together | Repository is intended for platform implementation and is currently empty | Rejected for this baseline |
| C. Store in `star-domains` | Could align with domain models | Product Delivery governance is not a business-domain implementation | Rejected |
| D. Create a new repository immediately | Strong isolation | Premature repository proliferation and unclear ownership | Deferred until a proven boundary requires it |
| E. Keep only in chat or local files | No setup cost | Not durable, reviewable or safely shareable | Rejected |

## Rationale and evidence

- The user explicitly approved the repository and path.
- `DEC-0020`–`DEC-0027` require durable Markdown and truthful synchronization claims.
- The working baseline is cross-cutting and currently best aligned with the architecture repository.
- Branch and Draft PR review preserve the distinction between synchronized, confirmed and frozen content.

## Consequences

### Expected benefits

- A stable authoritative location for versioned Product Delivery knowledge.
- Reviewable history through commits and pull requests.
- Clear separation between working branch content and approved `main` content.

### Trade-offs and risks accepted

- `star-architecture` may eventually become too broad.
- A later repository split will require link and ownership migration.
- GitHub remains unsuitable for live task, CRM, monitoring and financial state.

### Required follow-up work

- Keep `GITHUB_SYNC_STATUS.md` accurate.
- Reassess repository boundaries if the baseline grows into an independently maintained product.
- Do not merge Draft PR #1 until the documented review/validation gate is satisfied.

## Impact and relationships

- **Products / capabilities affected:** STAR architecture and Product Delivery knowledge.
- **Missions / work items affected:** Product Delivery foundation work.
- **Services / APIs / data affected:** none directly.
- **Teams / owners affected:** leadership, architecture, Product Delivery maintainers, AI collaborators and future reviewers.
- **Security / compliance / financial impact:** repository access and content classification must remain appropriate; secrets are prohibited.
- **Related decisions and artifacts:** `DEC-0025`, `DEC-0026`, `DEC-0027`, `GITHUB_SYNC_STATUS.md`, Draft PR #1.

## Validation

- **Success evidence:** all baseline files are visible on the dedicated branch and Draft PR, indexes remain aligned and no false synchronization claims occur.
- **Failure / revisit trigger:** repository ownership becomes unclear, unrelated material dominates the repository or access boundaries become inappropriate.
- **Measurement owner:** STAR architecture maintainers.
