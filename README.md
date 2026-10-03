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
│   ├── governance.md
│   ├── principles.md
│   └── standards.md
│
├── 02-architecture-vision/
│   ├── architecture-vision.md
│   └── stakeholders.md
│
├── 03-architecture-business/
│   ├── business-services.md
│   ├── capabilities.md
│   └── processes.md
│
├── 04-architecture-data/
│   ├── data-flow.md
│   ├── data-model.md
│   └── data-ownership.md
│
├── 05-architecture-application/
│   ├── application-landscape.md
│   ├── components.md
│   └── integration.md
│
├── 06-architecture-technology/
│   ├── deployment.md
│   ├── infrastructure.md
│   └── security.md
│
├── 07-architecture-solutions/
│   ├── solution-options.md
│   └── transition-architecture.md
│
├── 08-migration-roadmap/
│   ├── migration-waves.md
│   └── roadmap.md
│
├── 09-implementation-governance/
│   ├── architecture-review.md
│   └── exceptions.md
│
├── 10-decisions/
│   ├── ADR-001.md
│   ├── ADR-002.md
│   ├── ADR-003.md
│   └── requirements-management.md
│
├── 11-architecture-change/
│   ├── change-management.md
│   ├── change-request.md
│   └── impact-assessment.md
│
└── README.md
```

---

## 3. TOGAF ADM Mapping

| Your directory                 | TOGAF ADM     | Purpose                                        |
| ------------------------------ | ------------- | ---------------------------------------------- |
| `01-architecture-governance`   | Preliminary   | Architecture principles, standards, governance |
| `02-architecture-vision`       | Phase A       | Vision, scope, stakeholders, business drivers  |
| `03-architecture-business`     | Phase B       | Business architecture                          |
| `04-architecture-data`         | Phase C       | Data architecture                              |
| `05-architecture-application`  | Phase C       | Application architecture                       |
| `06-architecture-technology`   | Phase D       | Technology architecture                        |
| `07-architecture-solutions`    | Phase E       | Opportunities & Solutions                      |
| `08-migration-roadmap`         | Phase F       | Migration Planning                             |
| `09-implementation-governance` | Phase G       | Implementation Governance                      |
| `10-decisions`                 | Cross-cutting | Architecture Decision Records                  |
| —                              | Phase H       | Architecture Change Management                 |

### Requirements Management

Requirements Management is **continuous and central to the ADM**, rather than a single sequential phase. Requirements can enter, change, or be traced through every ADM phase.

---

## 4. Architecture Lifecycle

```text
                         ┌──────────────────────┐
                         │     Preliminary      │
                         │ Architecture         │
                         │ Capability/Governance │
                         └──────────┬───────────┘
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
                    ┌───────────────────────────────┐
                    │ C. Information Systems        │
                    │    ├── Data Architecture      │
                    │    └── Application Architecture│
                    └───────────────┬───────────────┘
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
                         ┌──────────────────────┐
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
                   └──────────── REST ──────────┘
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

1. **Business-driven architecture** — technology decisions should support measurable business outcomes.
2. **API-first integration** — application capabilities should be exposed through well-defined interfaces where appropriate.
3. **Security by design** — authentication, authorization, encryption, secrets management and auditability are architectural concerns.
4. **Separation of concerns** — presentation, business logic, data access and integration responsibilities should remain appropriately separated.
5. **Observability by design** — critical services should provide logs, metrics and operational visibility.
6. **Automation first** — repeatable build, test, deployment and infrastructure processes should be automated.
7. **Reuse before duplication** — existing approved capabilities should be reused where practical.
8. **Data ownership and accountability** — critical data should have identified ownership and stewardship.
9. **Resilience proportional to business criticality** — availability, backup and recovery controls should reflect business requirements.
10. **Architecture decisions are documented** — significant decisions should have traceable ADRs.

---

## 7. Source of Truth

| Concern | Source of truth |
|---|---|
| Implementation behavior | Application repositories |
| Database implementation | Database schema/migrations and approved database documentation |
| Deployment behavior | Deployment manifests, IaC and environment configuration |
| Runtime behavior | Approved production/runtime evidence |
| Architecture decisions | This architecture repository |
| Approved standards | Architecture governance documentation |
| Requirements | Requirements baseline/backlog and traceability records |

This repository must not silently replace implementation evidence.

---

## 8. Status Vocabulary

| Status | Meaning |
|---|---|
| **Confirmed** | Supported by available implementation/context evidence |
| **Proposed** | Target architecture recommendation requiring review/approval |
| **TBD** | Required information is not currently available |
| **To Validate** | A hypothesis that must be checked against implementation/runtime evidence |
| **Deprecated** | Previously accepted but no longer valid |
| **Approved** | Reviewed and formally accepted architecture decision |

---

## 9. Architecture Repository Rules

- Do not document assumptions as confirmed facts.
- Link architecture decisions to ADRs where practical.
- Keep As-Is and Target-State views separate.
- Record important exceptions explicitly.
- Review architecture when major business, technology, security or regulatory requirements change.
- Keep diagrams and textual descriptions consistent.
- Prefer traceability from **Business Requirement → Architecture Decision → Implementation → Outcome**.
