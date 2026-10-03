# Ads Promotional System — Enterprise Architecture

## 1. Purpose

This repository documents the Enterprise Architecture (EA) of the Ads Promotional System using a practical **TOGAF Architecture Development Method (ADM)**-aligned structure.

### Implementation applications

- **Backend:** `ads-promo-api`
- **Frontend:** `ads-promo-web`

The system scope currently covers advertisement, campaign and promotion management, customer management, reporting, audit, user/role/permission management, and customer messaging capabilities including WhatsApp-related functionality.

> **Architecture status:** Working architecture baseline.
>
> Items marked **Proposed**, **TBD**, or **To Validate** are not treated as confirmed implementation facts until they are verified against the source repositories, database schema, deployment configuration, integrations, and runtime environment.

---

## 2. Architecture Repository Structure

```text
enterprise-architecture/
│
├── 01-architecture-governance/
│   └── Readme.md
│
├── 02-architecture-vision/
│   └── Readme.md
│
├── 03-architecture-business/
│   └── Readme.md
│
├── 04-architecture-data/
│   └── Readme.md
│
├── 05-architecture-application/
│   └── Readme.md
│
├── 06-architecture-technology/
│   └── Readme.md
│
├── 07-architecture-solutions/
│   └── Readme.md
│
├── 08-migration-roadmap/
│   └── Readme.md
│
├── 09-implementation-governance/
│   └── Readme.md
│
├── 10-decisions/
│   ├── ADR-001.md
│   ├── ADR-002.md
│   ├── ADR-003.md
│   └── requirements-management.md
│
├── 11-architecture-change/
│   └── Readme.md
│
└── README.md
```

## 3. TOGAF ADM Mapping

| Repository                     | TOGAF ADM     | Primary purpose                                                         |
| ------------------------------ | ------------- | ----------------------------------------------------------------------- |
| `01-architecture-governance`   | Preliminary   | Establish architecture capability, principles, standards and governance |
| `02-architecture-vision`       | Phase A       | Define vision, scope, stakeholders and business drivers                 |
| `03-architecture-business`     | Phase B       | Define business capabilities, services and processes                    |
| `04-architecture-data`         | Phase C       | Define data architecture                                                |
| `05-architecture-application`  | Phase C       | Define application architecture                                         |
| `06-architecture-technology`   | Phase D       | Define technology architecture                                          |
| `07-architecture-solutions`    | Phase E       | Identify solution options and transition architectures                  |
| `08-migration-roadmap`         | Phase F       | Define migration strategy, roadmap and implementation waves             |
| `09-implementation-governance` | Phase G       | Govern implementation against approved architecture                     |
| `11-architecture-change`       | Phase H       | Manage architecture change and trigger new ADM work                     |
| `10-decisions`                 | Cross-cutting | Manage architecture decisions and requirements                          |

### Requirements Management

Requirements Management is **continuous and central to the ADM**, rather than a single sequential phase. Requirements can enter, change, or be traced through every ADM phase.

---

## 4. Architecture Lifecycle

```text
                         ┌───────────────────────┐
                         │     Preliminary       │
                         │ Architecture          │
                         │ Capability/Governance │
                         └──────────┬────────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │ A. Architecture      │
                         │ Vision               │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │ B. Business          │
                         │ Architecture         │
                         └──────────┬───────────┘
                                    │
                                    ▼
                    ┌────────────────────────────────┐
                    │ C. Information Systems         │
                    │    ├── Data Architecture       │
                    │    └── Application Architecture│
                    └───────────────┬────────────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │ D. Technology        │
                         │ Architecture         │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │ E. Opportunities &   │
                         │ Solutions            │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌───────────────────────┐
                         │ F. Migration          │
                         │ Planning              │
                         └──────────┬────────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │ G. Implementation    │
                         │ Governance           │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │ H. Architecture      │
                         │ Change Management    │
                         └──────────┬───────────┘
                                    │
                                    └──────► New / Updated ADM Cycle

              Requirements Management operates across all phases.
```

---

## 5. Application Boundary

```text
                         Ads Promotional System

                                  │
                   ┌──────────────┴──────────────┐
                   │                             │
                   ▼                             ▼
            ads-promo-web                 ads-promo-api
             Frontend/UI                    Backend/API
                   │                             │
                   └──────────── REST ───────────┘
                                  │
                                  ▼
                              Database
                                  │
                 ┌────────────────┼────────────────┐
                 │                │                │
                 ▼                ▼                ▼
              ERP/CRM        WhatsApp          Reporting/BI
             /External       /Messaging          /Analytics
```

> External integrations, database technology, deployment topology, and runtime components must be validated against the implementation repositories and environment before being treated as confirmed architecture.

---

## 6. Architecture Principles

The working architecture baseline follows these principles:

| #   | Architecture Principle                              | Description                                                                                                        |
| --- | --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| 1   | **Business-driven architecture**                    | Technology decisions should support measurable business outcomes.                                                  |
| 2   | **API-first integration**                           | Application capabilities should be exposed through well-defined interfaces where appropriate.                      |
| 3   | **Security by design**                              | Authentication, authorization, encryption, secrets management, and auditability are architectural concerns.        |
| 4   | **Separation of concerns**                          | Presentation, business logic, data access, and integration responsibilities should remain appropriately separated. |
| 5   | **Observability by design**                         | Critical services should provide logs, metrics, and operational visibility.                                        |
| 6   | **Automation first**                                | Repeatable build, test, deployment, and infrastructure processes should be automated.                              |
| 7   | **Reuse before duplication**                        | Existing approved capabilities should be reused where practical.                                                   |
| 8   | **Data ownership and accountability**               | Critical data should have identified ownership and stewardship.                                                    |
| 9   | **Resilience proportional to business criticality** | Availability, backup, and recovery controls should reflect business requirements.                                  |
| 10  | **Architecture decisions are documented**           | Significant decisions should have traceable Architecture Decision Records (ADRs).                                  |

---

## 7. Source of Truth

| Concern                 | Source of truth                                                |
| ----------------------- | -------------------------------------------------------------- |
| Implementation behavior | Application repositories                                       |
| Database implementation | Database schema/migrations and approved database documentation |
| Deployment behavior     | Deployment manifests, IaC and environment configuration        |
| Runtime behavior        | Approved production/runtime evidence                           |
| Architecture decisions  | This architecture repository                                   |
| Approved standards      | Architecture governance documentation                          |
| Requirements            | Requirements baseline/backlog and traceability records         |

This repository must not silently replace implementation evidence.

---

## 8. Status Vocabulary

| Status          | Meaning                                                                   |
| --------------- | ------------------------------------------------------------------------- |
| **Confirmed**   | Supported by available implementation/context evidence                    |
| **Proposed**    | Target architecture recommendation requiring review/approval              |
| **TBD**         | Required information is not currently available                           |
| **To Validate** | A hypothesis that must be checked against implementation/runtime evidence |
| **Deprecated**  | Previously accepted but no longer valid                                   |
| **Approved**    | Reviewed and formally accepted architecture decision                      |

---

## 9. Architecture Repository Rules

- Do not document assumptions as confirmed facts.
- Link architecture decisions to ADRs where practical.
- Keep As-Is and Target-State views separate.
- Record important exceptions explicitly.
- Review architecture when major business, technology, security or regulatory requirements change.
- Keep diagrams and textual descriptions consistent.
- Prefer traceability from **Business Requirement → Architecture Decision → Implementation → Outcome**.
