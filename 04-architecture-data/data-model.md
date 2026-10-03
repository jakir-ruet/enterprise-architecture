# Data Model

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
