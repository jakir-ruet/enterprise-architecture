# Data Architecture - Data Architecture Principles

| #   | Principle                  | Description                                                                                     |
| --- | -------------------------- | ----------------------------------------------------------------------------------------------- |
| 1   | **Data as an Asset**       | Business-critical data should be treated as an enterprise asset.                                |
| 2   | **Single Source of Truth** | Each critical data domain should have an identified authoritative source.                       |
| 3   | **Data Ownership**         | Critical data must have an accountable business owner.                                          |
| 4   | **Data Quality**           | Data should be accurate, complete, consistent, timely, and valid.                               |
| 5   | **Security by Design**     | Data security must be considered throughout the data lifecycle.                                 |
| 6   | **Least-Privilege Access** | Users and applications should receive only the data access required for their responsibilities. |
| 7   | **Data Minimization**      | Collect and retain only data required for legitimate business purposes.                         |
| 8   | **Traceability**           | Important data changes and movements should be traceable where required.                        |
| 9   | **Controlled Integration** | Data exchange between systems should use governed interfaces and contracts.                     |
| 10  | **Lifecycle Management**   | Data should have defined creation, usage, retention, archival, and disposal rules.              |

## 1. Data Model

## Logical Domain Model

```text
Customer
   │
   ├───────────────┐
   ▼               ▼
Campaign       Advertisement
   │               │
   ▼               ▼
Promotion        Media
   │
   ▼
Reporting / Audit

User ── Role ── Permission

Customer ── Messaging / WhatsApp
```

This is a logical model only.

The authoritative physical model must be derived from the actual database schema, migrations and application persistence mappings.

## Validation Required

- entity names
- primary/foreign keys
- cardinalities
- normalization
- sensitive data classification
- retention
- authoritative system for each domain

## 2. Data Ownership

## Working Ownership Model

| Data domain   | Candidate owner                 | Status      |
| ------------- | ------------------------------- | ----------- |
| Customer      | Business/customer domain        | To Validate |
| Advertisement | Advertisement business owner    | To Validate |
| Campaign      | Campaign business owner         | To Validate |
| Promotion     | Promotion business owner        | To Validate |
| Media         | Advertisement/media owner       | To Validate |
| User/Access   | Application/security owner      | To Validate |
| Audit         | Application/security/operations | To Validate |
| Messaging     | Messaging/business owner        | To Validate |

Ownership must be confirmed with business stakeholders.

## Governance

Each critical data domain should define:

- owner
- steward
- source of truth
- consumers
- classification
- retention
- quality expectations
- access policy

## 3. Data Flow

## High-Level Flow

```text
Users
  │
  ▼
ads-promo-web
  │
  ▼
ads-promo-api
  │
  ├──► Database
  │
  ├──► External Business Systems
  │
  ├──► Messaging / WhatsApp
  │
  └──► Reporting / BI
```

## Data Flow Principles

- Validate data at system boundaries.
- Protect sensitive data in transit and at rest.
- Avoid uncontrolled replication.
- Identify authoritative sources.
- Log appropriate audit events without exposing sensitive payloads unnecessarily.

Exact interfaces and data movement patterns are **To Validate**.
