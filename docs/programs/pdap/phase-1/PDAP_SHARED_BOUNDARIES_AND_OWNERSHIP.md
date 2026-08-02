# PDAP Shared Boundaries and Ownership

## Status

Leadership approved these boundaries as Candidate / minimum operating constraints for Phase 1. They are not final product architecture or technology-stack decisions.

## Shared Foundation admission rule

Shared Foundation accepts a capability only when:

1. two or more products demonstrate a real need;
2. semantics and lifecycle are materially consistent;
3. sharing reduces meaningful duplication, conflict or security risk;
4. ownership, compatibility and operations can be named;
5. the capability is not being generalized merely for possible future reuse.

Default rule: a capability remains product-owned until stable shared need is demonstrated. Extraction later occurs through ADR or RFC.

## Candidate Shared Foundation scope

Engineering foundations:

- repository bootstrap and module conventions;
- Git, branch, PR and merge controls;
- CI quality-control interfaces;
- environment naming and promotion model;
- secrets and configuration framework;
- logging, metrics and tracing integration conventions;
- audit-event envelope;
- deployment and rollback mechanisms;
- dependency and open-source governance;
- common security-control integration;
- documentation, ADR and RFC conventions.

Cross-product technical candidates requiring later evidence:

- Identity integration;
- Tenant-context propagation;
- authorization-policy interface;
- audit-trail envelope;
- API error, versioning and correlation conventions;
- webhook delivery primitives;
- connector lifecycle primitives;
- shared file/document metadata;
- notification primitives.

Default product-owned capabilities:

- SmartQuote Opportunity, Quote and Quote Version;
- SmartQuote pricing, Rule Center and approval semantics;
- GateHub onboarding and KYC orchestration;
- GateHub bank/PSP routing and connector-specific configuration;
- commercial pricing, cost and channel rules;
- product-specific UI, workflow and reporting.

## Merchant layered ownership model

| Concept | Candidate owner | Boundary |
|---|---|---|
| Merchant Identity | Shared / enterprise candidate | stable Merchant ID, Tenant linkage and common reference key |
| Merchant Commercial Profile | Missing | commercial attributes and product needs require later ownership decision |
| Merchant Onboarding / KYC Record | GateHub candidate | onboarding case, evidence, review and application lifecycle |
| Merchant Quote Reference | SmartQuote | minimum reference and controlled quotation snapshot |
| Merchant Operational Account | Out of current scope / Missing | activation, channel and production account state |

SmartQuote must not own complete Merchant master data. GateHub must not define legal or compliance policy authority. Production payment-account ownership is outside current PDAP scope.

## Core commercial-data ownership candidates

| Data | Candidate owner |
|---|---|
| Opportunity | SmartQuote |
| Quote | SmartQuote |
| Quote Version | SmartQuote |
| Pricing calculation result | SmartQuote |
| Pricing-rule snapshot | SmartQuote |
| Channel-cost snapshot used by a Quote Version | SmartQuote as immutable snapshot |
| Reusable channel-cost source | Missing commercial/channel source |
| Rule Center quotation rules | SmartQuote unless stable cross-product reuse is proven |
| Onboarding case | GateHub candidate |
| KYC/KYB evidence | GateHub or professional compliance source; unresolved |
| Bank/PSP application | GateHub candidate |
| Connector technical metadata | GateHub or shared connector capability; ADR/RFC required |
| Audit event semantics | Event-producing product; Shared Foundation may provide envelope and transport |

## Identity, Tenant and Security minimum boundary

Identity:

- products use a common identity source or controlled adapter;
- human, service, API-client and AI identities remain distinguishable;
- authentication and business authorization are separate;
- AI has no commercial approval, production-release or Gate-approval authority.

Tenant:

- every business record links to a defined Tenant;
- Tenant context propagates through APIs, events and audit records;
- UI parameters are not the sole enforcement mechanism;
- shared services declare tenant-aware or tenant-neutral behavior;
- Whitelabel and independent deployment preserve isolation;
- no difficult-to-reverse shared data model is created before the Tenant model is sufficiently bounded.

Authorization and data:

- products own business permission semantics;
- Shared Foundation may provide generic enforcement mechanisms;
- pricing, channel-cost, commercial exception and KYC access are independently controlled;
- approvals record actor, scope and decision evidence;
- administrator rights do not default across Tenants;
- data classifications include Public, Internal, Confidential Commercial and Restricted Customer/KYC/Payment;
- secrets do not enter code, Markdown, logs or AI conversations;
- production data is not used for unapproved development or AI processing.

This minimum boundary is an approved design input. Gate 1 remains not passed.