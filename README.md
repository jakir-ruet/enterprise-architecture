## [More about me](https://www.linkedin.com/in/jakir-ruet)

## Welcome to TOGAF Foundation Study Roadmap

|    # | Course Module                                  | What we will learn                                                    |
| ---: | ---------------------------------------------- | --------------------------------------------------------------------- |
|    1 | **Introduction to Enterprise Architecture**    | Enterprise, Architecture, EA, purpose, benefits                       |
|    2 | **Architecture Domains**                       | Business, Data, Application, Technology                               |
|    3 | **Architecture States**                        | Baseline, Target, Candidate, Transition, Resting                      |
|    4 | **Architecture Scope & Levels**                | Scope, depth, domains, time, Strategic/Segment/Capability             |
|    5 | **Architecture Partitioning & Abstraction**    | Partitions, Contextual, Conceptual, Logical, Physical                 |
|    6 | **Building Blocks**                            | BB, ABB, SBB                                                          |
|    7 | **TOGAF Standard**                             | Purpose, suitability, tailoring, structure                            |
|    8 | **Architecture Development Method (ADM)**      | ADM purpose and complete lifecycle                                    |
|    9 | **Preliminary Phase**                          | EA capability, principles, governance                                 |
|   10 | **Phase A — Architecture Vision**              | Vision, scope, stakeholders, Statement of Architecture Work           |
|   11 | **Phase B — Business Architecture**            | Business capabilities, processes, gap analysis                        |
|   12 | **Phase C — Information Systems Architecture** | Data + Application Architecture                                       |
|   13 | **Phase D — Technology Architecture**          | Technology infrastructure and platforms                               |
|   14 | **Phase E — Opportunities & Solutions**        | Solutions, transition architectures, roadmap                          |
|   15 | **Phase F — Migration Planning**               | Migration strategy and implementation planning                        |
|   16 | **Phase G — Implementation Governance**        | Architecture contracts, compliance                                    |
|   17 | **Phase H — Architecture Change Management**   | Change requests and continuous architecture                           |
|   18 | **Requirements Management + Applying ADM**     | Requirements, iteration, trade-offs                                   |
|   19 | **Content, Governance & Exam Preparation**     | Content Framework, Enterprise Continuum, Repository, governance, exam |

```bash
Enterprise Digital Employee Platform
│
├── Business Architecture
│   ├── Business Capability Map
│   ├── Business Processes
│   ├── Value Streams
│   └── Organization Model
│
├── Data Architecture
│   ├── Information Concepts
│   ├── Data Entities
│   ├── Data Model
│   └── Data Governance
│
├── Application Architecture
│   ├── Application Portfolio
│   ├── Application Services
│   ├── APIs
│   └── Integration Architecture
│
├── Technology Architecture
│   ├── Infrastructure
│   ├── Cloud
│   ├── Kubernetes
│   ├── Runtime
│   └── Network
│
├── Migration Roadmap
│
├── Architecture Governance
│
└── Architecture Repository
```

### Enterprise Architecture

It's a structured approach to aligning business strategy with technology, people, processes, applications, data, and infrastructure. The purpose is not simply to design IT systems, but to ensure that technology investments support business objectives, reduce complexity and risk, improve efficiency, and provide a scalable foundation for future growth.

Example:
Suppose a group has 20 companies using different ERP, HR, CRM, and reporting systems. As an Enterprise Architect, I would:

- Understand business capabilities.
- Inventory existing applications.
- Identify duplicated systems.
- Define common integration standards.
- Establish enterprise data ownership.
- Define target architecture.
- Create a phased modernization roadmap.

> The objective would not simply be "replace old systems." The objective would be business standardization, integration, security, scalability, and cost optimization.

### Need of Enterprise Architecture

According to your course, EA helps manage complexity and risk, support change, optimize processes, connect digital capabilities to changing business needs, balance transformation and operational efficiency, and enable enterprise-wide synergies.

- More effective strategic decision-making
- More effective and efficient business operations
- More effective digital transformation
- Better return on existing investment
- Reduced risk for future investment
- Faster and cheaper procurement
- Balancing conflicting demands

## The Open Group Architecture Framework (TOGAF)

It's a proven and widely used methodology and framework for developing enterprise architecture. It helps organizations design, evaluate, and build the right architecture to support their business goals.

It was first developed in 1995 based on a framework from the **US Department of Defense** and is maintained by **The Open Group**, a vendor-neutral consortium.

### Architecture Domains

TOGAF provides a structured approach to designing architecture across four key domains:

1. **Business Architecture:** Defines business strategy, governance, organization, and key processes.
2. **Data Architecture:** Describes the structure of logical and physical data assets.
3. **Application Architecture:** Provides a blueprint for individual application systems and their interactions.
4. **Technology Architecture:** Describes the software and hardware capabilities needed to support business, data, and application services.

#### Order to Cash Process (End to End) through Architecture Domain

![Order to Cash Process](/img/enterprise-architecture-layers.png)
![Order to Cash Process](/img/ordertocash-architecture-layers.png)

## 1. Purpose

This repository documents the Enterprise Architecture (EA) of the Ads Promotional System using a practical **TOGAF Architecture Development Method (ADM)**-aligned structure.

### Implementation applications

- **Backend:** `ads-promo-api`
- **Frontend:** `ads-promo-web`

The system scope currently covers advertisement, campaign and promotion management, customer management, reporting, audit, user/role/permission management, and customer messaging capabilities including WhatsApp-related functionality.

> **Architecture status:** Working architecture baseline.
>
> Items marked **Proposed**, ** To Be Determined (TBD)**, or **To Validate** are not treated as confirmed implementation facts until they are verified against the source repositories, database schema, deployment configuration, integrations, and runtime environment.

### To Be Determined (TBD) vs To Validate

| Term            | Meaning                                                                  | Example                               |
| --------------- | ------------------------------------------------------------------------ | ------------------------------------- |
| **TBD**         | The answer/decision has **not been determined yet**.                     | Production database: **TBD**          |
| **To Validate** | You have a proposed/assumed answer, but it **needs verification**.       | PostgreSQL is used: **To Validate**   |
| **Proposed**    | An architecture option/decision has been **suggested but not approved**. | API Gateway: **Proposed**             |
| **Confirmed**   | Evidence supports the information as **currently true**.                 | `ads-promo-api` exists: **Confirmed** |
| **Approved**    | The architecture decision has been **formally accepted**.                | ADR-001: **Approved**                 |

| Term                       | Meaning                                                                                               | When to Use                                                                                                                              | Example                             |
| -------------------------- | ----------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------- |
| **To Be Determined (TBD)** | The information or decision is **not known or decided yet**.                                          | Use when there is **no confirmed answer or decision available yet**.                                                                     | Production database: **TBD**        |
| **To Validate**            | An assumption or existing information is available, but it **needs to be verified** against evidence. | Use when you **think you know the answer**, but need to check the source repository, configuration, database, or production environment. | PostgreSQL is used: **To Validate** |
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
│   └── requirements-management.md
│
├── 11-architecture-change/
│   └── Readme.md
│
└── README.md
```

## 3. TOGAF ADM Mapping

| Repository                     | TOGAF ADM     | Primary Purpose                                                         | Example                                                                                                                          |
| ------------------------------ | ------------- | ----------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `01-architecture-governance`   | Preliminary   | Establish architecture capability, principles, standards and governance | Define **Business Alignment**, **API-First**, security principles, architecture standards and review process                     |
| `02-architecture-vision`       | Phase A       | Define vision, scope, stakeholders and business drivers                 | Define the vision for the **Ads Promotional System** and identify Business Owner, Marketing User, Management and IT stakeholders |
| `03-architecture-business`     | Phase B       | Define business capabilities, services and processes                    | **Campaign Management → Create Campaign → Approve Campaign → Publish Campaign**                                                  |
| `04-architecture-data`         | Phase C       | Define data architecture                                                | Define **Customer, Campaign, Advertisement, Promotion and Media** data domains, ownership and data flows                         |
| `05-architecture-application`  | Phase C       | Define application architecture                                         | Map **`ads-promo-web` → `ads-promo-api` → Database** and define application components and integrations                          |
| `06-architecture-technology`   | Phase D       | Define technology architecture                                          | Define the runtime, network, database, security, deployment, monitoring and infrastructure architecture                          |
| `07-architecture-solutions`    | Phase E       | Identify solution options and transition architectures                  | Compare **existing application enhancement vs modularization vs selective service extraction**                                   |
| `08-migration-roadmap`         | Phase F       | Define migration strategy, roadmap and implementation waves             | **Wave 1:** Security & Observability → **Wave 2:** API/Deployment Improvements → **Wave 3:** Modernization                       |
| `09-implementation-governance` | Phase G       | Govern implementation against approved architecture                     | Review whether an implementation follows approved **security, API, data and technology architecture**                            |
| `11-architecture-change`       | Phase H       | Manage architecture change and trigger new ADM work                     | Assess the impact of a **new business requirement, technology change or security requirement** and update the architecture       |
| `10-decisions`                 | Cross-cutting | Manage architecture decisions and requirements                          | API architecture decision; database decision; deployment decision                                                                |

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

### TOGAF Architecture Development Method (ADM)

![TOGAF Architecture Development Method (ADM)](/img/TOGAF-ADM-Architecture-Cycle.png)

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
