# PDAP Core Data and Security Register

## Core data ownership

| Data / record | Proposed owner | State |
|---|---|---|
| Merchant Identity | Shared/enterprise | Candidate; Gate 4 decision later |
| Merchant Commercial Profile | Business/commercial domain | Missing |
| Merchant Onboarding Case | GateHub | Candidate |
| KYC/KYB workflow state | GateHub | Candidate |
| Professional compliance decision | Compliance/Legal authority | Candidate boundary |
| Opportunity | SmartQuote | Candidate from confirmed scope |
| Quote | SmartQuote | Candidate from confirmed scope |
| Quote Version | SmartQuote | Candidate from confirmed scope |
| Pricing result | SmartQuote | Candidate |
| Quotation rule snapshot | SmartQuote | Candidate |
| Channel-cost snapshot | SmartQuote | Confirmed requirement |
| Reusable channel-cost source | Commercial/channel source | Missing; must close before Gate 2 disposition |
| Bank/PSP application | GateHub | Candidate |
| Connector lifecycle | GateHub | Candidate |
| Connector technical primitives | Shared Foundation possible | Candidate overlap |
| Production credential | Secrets/operations system | Candidate |
| Operational payment account | Future payment/operations domain | Missing |

## Identity, Tenant and authorization

- Identity source and authentication: shared/external candidate.
- Tenant ID: enterprise/shared candidate.
- Tenant context must propagate through API, event and audit evidence.
- Each product enforces tenant isolation and product-specific authorization semantics.
- Shared Foundation may provide enforcement primitives but does not own product permissions.
- Administrative access is not cross-tenant by default.
- AI has no commercial approval, KYC approval, production release, Gate passage or Product Commitment authority.

## Data classification

- Public;
- Internal;
- Confidential commercial;
- Restricted customer/KYC/payment.

SmartQuote pricing, channel cost and commercial exceptions are Confidential. GateHub KYC, bank documents and personal information are Restricted.

## Security boundaries

- secrets stay outside source code, Markdown, logs and AI conversations;
- production data is not used for unapproved development or AI processing;
- provider credentials use external secret references where possible;
- logs redact sensitive payloads by default;
- audit evidence includes actor, tenant, action, record, timestamp, result and correlation;
- restricted-data retention, deletion and residency remain Missing pending professional authority;
- professional security, Compliance and Legal validation remains a later trigger.

## Status

These are approved design inputs and Candidate ownership records. They are not final security architecture and do not pass Gate 1, Gate 2, Gate 3 or Gate 4.