# PDAP GateHub Gate 3 Package

## Status

- Recommendation: Recovery required.
- Gate 3: not passed.
- GateHub Delivery: not started.
- Target 2026-08-10 remains At risk.

## Candidate authority boundary

GateHub is a Candidate capability for Merchant onboarding, KYC/KYB workflow state, bank/PSP applications, connector onboarding, certification evidence, capability/status query and audit evidence.

The first stage excludes real-time payment routing, transaction execution, settlement, ledger, reconciliation, full fraud engine, SmartQuote pricing, universal document management, autonomous AI KYC approval and plaintext secret storage.

## Professional authority boundary

GateHub manages workflow and evidence state. It does not create legal or regulatory rules and does not replace Compliance or Legal judgment. Professional decisions must retain their authoritative source and reviewer evidence.

## Candidate ownership

| Record | Candidate owner |
|---|---|
| Merchant Identity | Shared/enterprise candidate; Gate 4 decision later |
| Merchant Commercial Profile | Missing |
| Merchant Onboarding/KYC | GateHub |
| Bank/PSP application | GateHub |
| Connector onboarding/lifecycle | GateHub |
| Connector technical primitives | Shared Foundation possible overlap |
| Professional compliance decision | Compliance/Legal authority |
| Production credential | Approved secrets/operations system |
| Quote/Opportunity | SmartQuote |

## Candidate components

- Merchant Reference Adapter;
- Onboarding Case;
- Evidence/Document Reference;
- KYC/KYB Workflow;
- Compliance Decision Reference;
- Bank/PSP Application;
- Connector Registry and Onboarding;
- Capability Catalogue;
- Certification Evidence;
- API/Integration;
- Audit and Notification/Task Coordination.

These are logical candidates, not approved product architecture or microservice decomposition.

## Connector and credential boundary

Candidate lifecycle: Proposed, Information Required, Configuration Prepared, Test/Certification, Ready, Enabled, Suspended and Retired.

GateHub may retain secret references, credential status, rotation metadata, environment binding and audit references. Plaintext credentials, unrestricted private keys, passwords and uncontrolled production secrets remain prohibited.

## SmartQuote dependency

GateHub may provide onboarding readiness, available bank/PSP/channel references, supported capability metadata, connector readiness and approved availability state. SmartQuote consumes controlled references and status only; it must not receive unrestricted KYC documents, personal data, credentials or compliance notes.

## Candidate first slice

`Merchant Reference -> Onboarding Case -> Minimum Evidence Checklist -> Internal Review State -> One Bank/PSP Application -> One Connector Readiness Record -> Capability/Status Query -> Audit Evidence`

This slice does not include payment routing or transaction execution.

## Remaining recovery conditions

- leadership disposition of the Candidate package;
- authoritative Compliance/Legal source;
- Merchant and connector ownership;
- repository and environment disposition;
- one bounded bank/PSP scenario;
- restricted-data and credential review;
- minimum API and first-slice acceptance;
- Gate 4 material-conflict disposition.

## Recommendation

Recovery required. This package does not pass Gate 3 or authorize architecture approval, Commitment, implementation or Delivery.