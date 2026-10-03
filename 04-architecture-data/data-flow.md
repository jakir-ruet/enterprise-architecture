# Data Flow

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
