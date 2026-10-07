## [More about me](https://www.linkedin.com/in/jakir-ruet)

## Welcome to TOGAF Foundation Study Roadmap

|      # | Course Module                                 | What we will learn                                                                                                      |
| -----: | --------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
|  **1** | **Introduction to Enterprise Architecture**   | Enterprise Architecture definition, purpose & benefits                                                                  |
|  **2** | **Architecture Domains**                      | Domains, Levels, Partitions & Abstractions                                                                              |
|  **3** | **Architecture Development Method (ADM)**     | ADM phases, Artifacts & Deliverables, Building Blocks, Stakeholders, Concerns, Viewpoints & Views                       |
|  **4** | **Preliminary Phase**                         | Purpose, Objectives, Steps & Approach, Architecture Principles                                                          |
|  **5** | **Phase A: Architecture Vision**              | Statement of Architecture Work, Business Transformation Readiness Assessment, Architecture Vision & Definition Document |
|  **6** | **Phase B: Business Architecture**            | Purpose, Objectives, Steps & Approach, Gap Analysis                                                                     |
|  **7** | **Phase C: Information Systems Architecture** | Purpose, Objectives, Steps & Approach, Application & Data Architecture Artifacts                                        |
|  **8** | **Phase D: Technology Architecture**          | Purpose, Objectives, Steps & Approach, Technology Architecture Artifacts                                                |
|  **9** | **Phase E: Opportunities and Solutions**      | Interoperability & Risk Management, Architecture Roadmap, Implementation and Migration Plan                             |
| **10** | **Phase F: Migration Planning**               | Purpose, Objectives, Steps & Approach, Implementation Governance Model                                                  |
| **11** | **Phase G: Implementation Governance**        | Architecture Contracts, Compliance Assessment, Support of Agile Software Development                                    |
| **12** | **Phase H: Architecture Change Management**   | Purpose, Objectives, Steps & Approach, Change Request                                                                   |
| **13** | **Requirements Management Phase**             | Purpose, Objectives, Steps & Approach, Requirements Impact Assessment                                                   |
| **14** | **Applying the ADM**                          | ADM Techniques & Iterations, Information Flow, Architecture Alternatives & Trade-off Method                             |
| **15** | **Content & Core Concepts**                   | Content Framework & Enterprise Metamodel, Enterprise Continuum, Architecture Repository                                 |
| **16** | **Architecture Governance & EA Capability**   | Corporate & EA Governance, Architecture Board & Capability                                                              |
| **17** | **Exam Preparation & Definitions**            | Key Definitions, Exam Preparation & Time Management, Question Analysis & Answer Selection                               |
| **18** | **Practice Test**                             | TOGAF EA Part 1 Sample Exam, 40 Questions, Answers & Explanations                                                       |
| **19** | **Wrap-up**                                   | Next Steps & Course Materials                                                                                           |

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

## 1. Introduction to Enterprise Architecture

**The Open Group Architecture Framework (TOGAF)** is a proven and widely used methodology and framework for developing enterprise architecture. It helps organizations design, evaluate, and build the right architecture to support their business goals. It was first developed in 1995 based on a framework from the **US Department of Defense** and is maintained by **The Open Group**, a vendor-neutral consortium.

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

### Need/Purpose of Enterprise Architecture

According to your course, EA helps manage complexity and risk, support change, optimize processes, connect digital capabilities to changing business needs, balance transformation and operational efficiency, and enable enterprise-wide synergies.

- More effective strategic decision-making
- More effective and efficient business operations
- More effective digital transformation
- Better return on existing investment
- Reduced risk for future investment
- Faster and cheaper procurement
- Balancing conflicting demands

### Benefits of Enterprise Architecture

| #     | Benefit                                              | What it means                                                                                                     |
| ----- | ---------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| **1** | **More effective strategic decision-making**         | Gives leadership an enterprise-wide view for making better architecture and investment decisions.                 |
| **2** | **More effective and efficient business operations** | Helps identify duplication, inefficiencies, and opportunities to improve business processes.                      |
| **3** | **More effective digital transformation**            | Connects digital initiatives with business needs and the target architecture.                                     |
| **4** | **Better return on existing investment**             | Helps organizations maximize the value of existing applications, data, and technology investments.                |
| **5** | **Reduced risk for future investment**               | Architecture principles, standards, and roadmaps reduce the risk of making inappropriate technology investments.  |
| **6** | **Faster and cheaper procurement**                   | Reusable standards, reference architectures, and defined technology choices can simplify procurement.             |
| **7** | **Balancing conflicting demands**                    | Helps balance competing requirements such as cost, security, agility, business needs, and technology constraints. |

## 2. Architecture Domains

TOGAF provides a structured approach to designing architecture across four key domains:

1. **Business Architecture:** Defines business strategy, governance, organization, and key processes.
2. **Data Architecture:** Describes the structure of logical and physical data assets.
3. **Application Architecture:** Provides a blueprint for individual application systems and their interactions.
4. **Technology Architecture:** Describes the software and hardware capabilities needed to support business, data, and application services.

### Order to Cash Process (End to End) through Architecture Domain

![Order to Cash Process](/img/enterprise-architecture-layers.png)
![Order to Cash Process](/img/ordertocash-architecture-layers.png)

## 3. Architecture Development Method (ADM)

ADM provides a structured cycle for moving an enterprise from its current architecture (Baseline) toward its desired future architecture (Target). The basic idea

```bash
Current State
   │
   │  ADM
   ↓
Architecture Development
   │
   ↓
Target State
   │
   ↓
Implementation & Governance
   │
   ↓
Change Management
   │
   └──────────────→ New Architecture Cycle
```

**ADM Phases** The ADM consists of a series of phases. The major flow is:

```bash
                ┌─────────────────────┐
                │ Preliminary Phase   │
                └──────────┬──────────┘
                            ↓
                ┌─────────────────────┐
                │ Phase A             │
                │ Architecture Vision │
                └──────────┬──────────┘
                            ↓
            ┌───────────────┴───────────────┐
            ↓                               ↓
    ┌─────────────┐                 ┌─────────────┐
    │ Phase B     │                 │ Phase C     │
    │ Business    │                 │ Information │
    │ Architecture│                 │ Systems     │
    └──────┬──────┘                 └──────┬──────┘
            └───────────────┬───────────────┘
                            ↓
                ┌─────────────────────┐
                │ Phase D             │
                │ Technology          │
                │ Architecture        │
                └──────────┬──────────┘
                            ↓
                ┌─────────────────────┐
                │ Phase E             │
                │ Opportunities &     │
                │ Solutions           │
                └──────────┬──────────┘
                            ↓
                ┌─────────────────────┐
                │ Phase F             │
                │ Migration Planning  │
                └──────────┬──────────┘
                            ↓
                ┌─────────────────────┐
                │ Phase G             │
                │ Implementation      │
                │ Governance           │
                └──────────┬──────────┘
                            ↓
                ┌─────────────────────┐
                │ Phase H             │
                │ Architecture Change │
                │ Management          │
                └──────────┬──────────┘
                            │
                            └──────→ New ADM cycle
```

**The Most Important Concept**

| Step                       | Logic / Key Question                                      | ADM Phase                                      | Main Focus                                                                                  |
| -------------------------- | --------------------------------------------------------- | ---------------------------------------------- | ------------------------------------------------------------------------------------------- |
| **1. Prepare**             | **Can we do architecture effectively?**                   | **Preliminary Phase**                          | Establish the Architecture Capability, governance, principles, organization, and approach   |
| **2. Establish Direction** | **Where do we want to go?**                               | **Phase A — Architecture Vision**              | Define the vision, scope, stakeholders, and desired future direction                        |
| **3. Design**              | **What should the future enterprise look like?**          | **Phase B — Business Architecture**            | Define the Target Business Architecture                                                     |
|                            |                                                           | **Phase C — Information Systems Architecture** | Define **Data & Application Architecture**                                                  |
|                            |                                                           | **Phase D — Technology Architecture**          | Define the Target Technology Architecture                                                   |
| **4. Plan the Change**     | **How do we get there?**                                  | **Phase E — Opportunities & Solutions**        | Identify solution options, transition architectures, and major implementation opportunities |
|                            |                                                           | **Phase F — Migration Planning**               | Develop migration strategy, roadmap, and implementation plan                                |
| **5. Implement**           | **Are we implementing according to the architecture?**    | **Phase G — Implementation Governance**        | Govern implementation and ensure compliance with the approved architecture                  |
| **6. Manage Change**       | **What happens when the business or technology changes?** | **Phase H — Architecture Change Management**   | Manage architecture changes and determine when a new ADM cycle is required                  |
| **Continuous**             | **Are requirements still valid and being addressed?**     | **Requirements Management**                    | Identify, assess, track, and manage requirements throughout the ADM cycle                   |

> Easy way to remember: `Prepare → Direction → Design → Plan → Implement → Change`

**ADM vs Architecture Domains**

| Aspect                   | Architecture Domains                                          | ADM                                                                          |
| ------------------------ | ------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| **Fundamental question** | **What are we architecting?**                                 | **How do we develop the architecture?**                                      |
| **Purpose**              | Organize the architecture into major areas                    | Provide the method/process for developing and managing architecture          |
| **Main components**      | Business, Data, Application, Technology                       | Preliminary, A, B, C, D, E, F, G, H                                          |
| **Business**             | Business Architecture                                         | **Phase B** develops Business Architecture                                   |
| **Data**                 | Data Architecture                                             | **Phase C** develops Data Architecture                                       |
| **Application**          | Application Architecture                                      | **Phase C** develops Application Architecture                                |
| **Technology**           | Technology Architecture                                       | **Phase D** develops Technology Architecture                                 |
| **Nature**               | Architecture **content / subject areas**                      | Architecture **development method / process**                                |
| **Example**              | Customer Management, Employee Management, Technology Platform | Define Vision → Design Architecture → Plan Migration → Govern Implementation |
| **Relationship**         | Defines **what areas** the architecture covers                | Defines **how and when** those areas are developed                           |
| **Exam keyword**         | **What**                                                      | **How**                                                                      |

### Artifacts, Deliverables & Building Blocks

These three terms are important because they describe what is produced during architecture development. The three concepts.

| Concept            | Meaning                                                                       | Simple Question                   |
| ------------------ | ----------------------------------------------------------------------------- | --------------------------------- |
| **Deliverable**    | A formally reviewed and agreed work product that is delivered to stakeholders | **What do we deliver?**           |
| **Artifact**       | A work product that describes some aspect of the architecture                 | **What do we document?**          |
| **Building Block** | A reusable component of business, IT, or architecture capability              | **What can we reuse/build with?** |

#### Deliverable

A deliverable is a formally reviewed output that is agreed with stakeholders and usually represents the completion of significant architecture work.

| Deliverable                      | Purpose                                                       |
| -------------------------------- | ------------------------------------------------------------- |
| Architecture Definition Document | Describes the architecture                                    |
| Architecture Vision              | Communicates the desired architectural direction              |
| Architecture Roadmap             | Shows how the enterprise moves toward the Target Architecture |
| Implementation & Migration Plan  | Defines how implementation will be performed                  |

```bash
Architecture Work
       ↓
Analysis
       ↓
Documentation
       ↓
Review
       ↓
Agreement
       ↓
DELIVERABLE
```

> A deliverable is therefore more than just an informal document.

#### Artifact

An artifact is a work product that describes an aspect of the architecture. Artifacts can generally be categorized as:

| Artifact Category | Focus                                     | Example                           |
| ----------------- | ----------------------------------------- | --------------------------------- |
| **Catalog**       | Lists things                              | Application Portfolio Catalog     |
| **Matrix**        | Shows relationships                       | Application/Data Matrix           |
| **Diagram**       | Shows structure or relationships visually | Application Communication Diagram |

```bash
Application       Data
-------------------------
Employee Service  Employee
Leave Service     Leave
Payroll Service   Payroll
```

#### Building Block

Building Block represents a potentially reusable component of an architecture. Think of it as a piece from which an architecture can be constructed.

```bash
Enterprise Digital Employee Platform
│
├── Authentication Building Block
├── Employee Management Building Block
├── Leave Management Building Block
├── Notification Building Block
├── API Gateway Building Block
└── Audit Logging Building Block
```

> In stead of designing everything from scratch, the organization can reuse approved building blocks.

### Architecture Building Blocks vs Solution Building Blocks

This distinction is useful in TOGAF.

| Type                                  | Meaning                                        | Example                                                        |
| ------------------------------------- | ---------------------------------------------- | -------------------------------------------------------------- |
| **Architecture Building Block (ABB)** | Defines **what capability is required**        | Authentication capability                                      |
| **Solution Building Block (SBB)**     | Defines **how that capability is implemented** | Keycloak, Microsoft Entra ID, or another approved IAM solution |

> - ABB > What is needed
> - SBB > How it is implemented

### Stakeholders, Concerns, Viewpoints & Views

Different stakeholders need different views of the same architecture.

#### Stakeholder

A stakeholder is a person, team, organization, or group that has an interest in the architecture or is affected by it. For an Enterprise Digital Employee Platform, stakeholders could include:

| Stakeholder                | Main Interest                              |
| -------------------------- | ------------------------------------------ |
| CEO / Executive Management | Business value, investment, transformation |
| HR                         | Employee processes and capabilities        |
| Finance                    | Payroll and financial data                 |
| IT Management              | Architecture, cost, operations             |
| Enterprise Architect       | Overall architecture alignment             |
| Security Team              | Security, compliance, risk                 |
| Developers                 | Application design and APIs                |
| Operations Team            | Infrastructure, availability, monitoring   |
| Employees                  | Usability and employee services            |

#### Concern

A concern is something important to a stakeholder that the architecture needs to address.
Different stakeholders have different concerns.

| Stakeholder          | Example Concern             |
| -------------------- | --------------------------- |
| CEO                  | Business value              |
| CFO                  | Cost / ROI                  |
| HR                   | Process efficiency          |
| Security Team        | Security and compliance     |
| Enterprise Architect | Architecture consistency    |
| Developer            | API and application design  |
| Operations           | Availability and monitoring |
| Employee             | Usability and performance   |

#### Viewpoint

A viewpoint defines how an architecture will be viewed to address particular stakeholder concerns.
Think of it as a template or perspective for creating a view.

| Concept         | Meaning                                                         |
| --------------- | --------------------------------------------------------------- |
| **Stakeholder** | Who is interested?                                              |
| **Concern**     | What do they care about?                                        |
| **Viewpoint**   | How should we look at the architecture to address that concern? |
| **View**        | The actual representation produced using that viewpoint         |

#### View

A view is the actual representation of the architecture from a particular viewpoint.
For example, a security stakeholder may need a security view.

```bash
Security View
     ↓
Identity
     ↓
Authentication
     ↓
Authorization
     ↓
Encryption
     ↓
Audit
```

## 4. Preliminary Phase

The primary purpose is to create and establish the Architecture Capability of the enterprise. this module covers.

1. Purpose, Objectives, Steps & Approach
2. Architecture Principles

**Architecture Capability** is the organization's ability to perform, govern, maintain, and use Enterprise Architecture effectively.
It involves areas such as:

| Area             | What needs to be established          |
| ---------------- | ------------------------------------- |
| **Organization** | EA team and responsibilities          |
| **Governance**   | Architecture governance structure     |
| **Principles**   | Architecture principles               |
| **Processes**    | Architecture processes                |
| **People**       | Required skills and roles             |
| **Tools**        | Architecture tools and repositories   |
| **Methods**      | TOGAF and other applicable methods    |
| **Standards**    | Architecture and technology standards |
| **Resources**    | Budget, time and supporting resources |

**Objectives of the Preliminary** Phase the Preliminary Phase has two broad objectives:

1. Objective 1: Determine the desired Architecture Capability for the enterprise.
2. Objective 2: Establish the Architecture Capability.

> This means we first determine what capability is needed, then establish the organizational capability to deliver it.

**Major Activities** The Preliminary Phase addresses several important activities.

| Activity                                     | Purpose                                                               |
| -------------------------------------------- | --------------------------------------------------------------------- |
| **Review organizational context**            | Understand the enterprise and its environment                         |
| **Scope affected organizations**             | Determine which parts of the enterprise are involved                  |
| **Identify existing frameworks and methods** | Understand existing EA, governance and management approaches          |
| **Set architecture maturity target**         | Determine the desired level of architecture capability                |
| **Define EA organizational model**           | Establish roles, responsibilities and organizational structure        |
| **Define architecture governance**           | Establish how architecture decisions will be governed                 |
| **Identify resources**                       | Determine people, budget, tools and other resources                   |
| **Select architecture tools**                | Establish tools for modeling, documentation and repository management |
| **Define architecture principles**           | Establish guiding principles for architecture decisions               |
| **Tailor the TOGAF framework**               | Adapt TOGAF to the organization's context                             |

**Preliminary Phase — Overall Flow**

```bash
Understand Enterprise Context
          ↓
Identify Drivers & Requirements
          ↓
Determine Architecture Work Requirements
          ↓
Define Architecture Principles
          ↓
Select / Tailor Architecture Framework
          ↓
Define EA Organization
          ↓
Establish Governance
          ↓
Evaluate / Define Architecture Capability
          ↓
Architecture Capability Established
          ↓
       Phase A
```

Let's apply this to your **Enterprise Digital Employee Platform**. Suppose an organization wants to create an enterprise-wide employee platform. Before designing the platform, we shouldn't immediately start drawing microservices. We first establish the architecture capability.

| Preliminary Activity   | Digital Employee Platform Example                              |
| ---------------------- | -------------------------------------------------------------- |
| Organizational context | HR, Finance, IT, Security and business units                   |
| Scope                  | Employee management across the enterprise                      |
| Stakeholders           | HR, CIO, Finance, Security, IT Operations                      |
| EA organization        | Enterprise Architect + Solution Architects + Domain Architects |
| Governance             | Architecture Review Board                                      |
| Principles             | Security by design, API-first, reuse before duplication        |
| Standards              | Java, Spring Boot, Oracle, API standards, security standards   |
| Tools                  | Architecture repository and modeling tools                     |
| Architecture maturity  | Assess current EA maturity and define target                   |
| Framework              | Tailor TOGAF to organizational requirements                    |

**Preliminary Phase vs Phase A**

| Preliminary Phase                   | Phase A                                         |
| ----------------------------------- | ----------------------------------------------- |
| **Prepares the organization**       | **Starts the specific architecture initiative** |
| Establishes Architecture Capability | Establishes Architecture Vision                 |
| Defines governance                  | Defines project/initiative scope                |
| Establishes principles              | Defines stakeholder expectations                |
| Defines EA organization             | Creates Statement of Architecture Work          |
| Tailors the framework               | Develops Architecture Vision                    |
| Establishes methods and tools       | Assesses transformation readiness               |

> - Easy memory
> - Preliminary = Prepare the architecture capability
> - Phase A = Start and define the architecture initiative

#### Architecture Principles

Without principles, different teams may make different decisions.

| Situation       | Without Principles                  | With Principles                        |
| --------------- | ----------------------------------- | -------------------------------------- |
| API development | Every team chooses its own approach | Common API standards                   |
| Security        | Security added later                | Security considered from the beginning |
| Technology      | Teams select different technologies | Approved technology standards          |
| Data            | Multiple sources of truth           | Defined data ownership                 |
| Applications    | Duplicate solutions                 | Reuse existing capabilities            |
| Operations      | Monitoring added later              | Observability designed into services   |

#### Characteristics of Good Architecture Principles

A good principle should be

| Characteristic  | Meaning                                            |
| --------------- | -------------------------------------------------- |
| **Clear**       | Easy to understand                                 |
| **Consistent**  | Does not conflict with other principles            |
| **Stable**      | Should remain valid for a reasonable period        |
| **Actionable**  | Can actually guide decisions                       |
| **Relevant**    | Supports enterprise objectives                     |
| **Enforceable** | Can be used in governance and architecture reviews |

For your Enterprise Digital Employee Platform, we could define

| ID         | Principle                                       | Statement                                                                                                         |
| ---------- | ----------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| **BP-001** | Business-driven architecture                    | Architecture decisions must support measurable business outcomes.                                                 |
| **BP-002** | Capability alignment                            | Applications and technology must align with required business capabilities.                                       |
| **BP-003** | API-first integration                           | Application capabilities should be exposed through well-defined interfaces where appropriate.                     |
| **BP-004** | Security by design                              | Security must be treated as an architectural concern throughout the lifecycle.                                    |
| **BP-005** | Separation of concerns                          | Presentation, business logic, data access and integration responsibilities should remain appropriately separated. |
| **BP-006** | Observability by design                         | Critical services should provide logs, metrics and operational visibility.                                        |
| **BP-007** | Automation first                                | Repeatable build, test, deployment and infrastructure processes should be automated.                              |
| **BP-008** | Reuse before duplication                        | Existing approved capabilities should be reused where practical.                                                  |
| **BP-009** | Data ownership and accountability               | Critical data should have identified ownership and stewardship.                                                   |
| **BP-010** | Resilience proportional to business criticality | Availability, backup and recovery controls should reflect business requirements.                                  |

## 5. Phase A: Architecture Vision

## 6. Phase B: Business Architecture

## 7. Phase C: Information Systems Architecture

## 8. Phase D: Technology Architecture

## 9. Phase E: Opportunities and Solutions

## 10. Phase F: Migration Planning

## 11. Phase G: Implementation Governance

## 12. Phase H: Architecture Change Management

## 13. Requirements Management Phase

## 14. Applying the ADM

## 15. Content & Core Concepts

## 16. Architecture Governance & EA Capability

## 17. Exam Preparation & Definitions

## 18. Practice Test

## 19. Wrap-up

---

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
