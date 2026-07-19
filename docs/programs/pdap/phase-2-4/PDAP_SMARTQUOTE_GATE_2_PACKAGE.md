# PDAP SmartQuote Gate 2 Package

## Status

- Recommendation: Conditional pass candidate.
- Gate 2: not passed.
- M1: not passed.
- M001: not Committed.
- SmartQuote Delivery: not started.
- Target 2026-08-03 remains At risk.

## Confirmed Mission boundary

SmartQuote covers Merchant reference, multiple Opportunities per Merchant, Quote, Quote Version retention, pricing inputs, frozen pricing/rule/channel-cost snapshots, Rule Center, approval, issuance, API query and audit evidence. It excludes complete CRM, Merchant Onboarding/KYC, payment execution, settlement, ledger, general-purpose workflow/rule platforms and autonomous AI commercial approval.

## Candidate architecture package

System context includes internal sales, presales, pricing, approval and operations users plus future CRM, Merchant Portal and partner API clients.

Candidate logical components:

- Merchant Reference Adapter;
- Opportunity Management;
- Quote Lifecycle;
- Quote Version Store;
- Pricing Evaluation;
- Rule Center;
- Approval;
- Issuance/Rendering;
- API;
- Audit/Evidence;
- Integration Adapters.

These are logical boundaries, not a deployment topology or microservice approval.

## System-of-record candidates

| Record | Candidate owner |
|---|---|
| Opportunity | SmartQuote |
| Quote | SmartQuote |
| Quote Version | SmartQuote |
| Frozen pricing/rule snapshot | SmartQuote |
| Frozen channel-cost snapshot | SmartQuote |
| Reusable channel-cost source | Missing commercial/channel source |
| Merchant Identity | Shared/enterprise candidate |
| Merchant Commercial Profile | Missing |
| KYC/onboarding | GateHub candidate |

Merchant Identity remains for Gate 4 disposition. Reusable channel-cost source ownership must close before actual Gate 2 disposition.

## API and snapshot boundary

Candidate API capabilities include Merchant reference query, Opportunity create/query, Quote creation, Quote Version generation, submit/approve/reject, issuance, version query and decision-evidence retrieval. Material writes should be idempotent, tenant-bound, authorized and auditable.

Every Quote Version must retain rule identifiers/versions, effective parameters, pricing inputs/results, selected channel-cost values, source reference, evaluation time, actor/system and approval evidence. Later source changes must not mutate prior versions.

## Security and deployment direction

Opportunity, Quote and Quote Version are tenant-bound. Pricing, channel cost and commercial exceptions are Confidential. Identity and authorization remain separate, least privilege applies, sensitive values stay out of ordinary logs, and audit records include actor, tenant, record, action, result and time.

Candidate direction supports independent deployment, Whitelabel configuration, versioned APIs, isolated adapters and reversible schema evolution without requiring early microservices or multi-region architecture.

## First delivery slice

`Merchant Reference -> Opportunity -> Quote -> Quote Version -> Pricing/Rule Snapshot -> Approval -> Issuance -> API Query`

Evidence must include one Merchant with multiple Opportunities, V1/V2/V3 retention, frozen pricing and channel-cost snapshot, permission/approval evidence, API/error behavior, QA evidence and Product Owner plus named business acceptance.

## Conditions before actual disposition

- Merchant and reusable channel-cost source ownership;
- product repository and environment disposition;
- minimum API contract evidence;
- data classification and access model;
- component-boundary review;
- test ownership;
- deployment/rollback direction;
- Gate 4 material-conflict review;
- separate M1 and Product Commitment.

## Recommendation

Conditional pass candidate only. This does not pass Gate 2 or authorize M1, Commitment, implementation or Delivery.