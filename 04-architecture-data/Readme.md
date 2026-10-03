# Data Architecture

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
