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

A succinct description of the Target Architecture that describes its business value and the changes to the enterprise that will result from its successful deployment. It serves as an aspirational vision and a boundary for detailed architecture development. Key Deliverables in Phase A

1. Statement of Architecture Work
2. Business Transformation Readiness Assessment
3. Architecture Vision & Definition Document

The Statement of Architecture Work defines what architecture work is going to be performed, why it is being performed, and what the architecture effort will cover.

| Aspect                  | Architecture Vision                             |
| ----------------------- | ----------------------------------------------- |
| **Level**               | High-level                                      |
| **Focus**               | Future / Target Architecture                    |
| **Purpose**             | Communicate the desired architectural direction |
| **Describes**           | Capabilities and business value                 |
| **Includes**            | Target Architecture value propositions and KPIs |
| **Considers**           | Business transformation risks and mitigation    |
| **Stakeholder purpose** | Create a common understanding and support       |
| **ADM Phase**           | **Phase A — Architecture Vision**               |

Don't confuse it with the Statement of Architecture Work

| Statement of Architecture Work         | Architecture Vision                            |
| -------------------------------------- | ---------------------------------------------- |
| Defines **the architecture work**      | Defines **the architectural direction**        |
| Scope, approach, deliverables          | Capabilities, value, Target Architecture       |
| **What architecture work will we do?** | **What will the future architecture achieve?** |

Suppose we are implementing your Digital Employee Platform.

| Readiness Factor   | Current Situation                  | Readiness | Risk   | Mitigation                     |
| ------------------ | ---------------------------------- | --------- | ------ | ------------------------------ |
| Leadership support | Strong                             | High      | Low    | Continue executive sponsorship |
| Employee adoption  | Employees used to legacy systems   | Medium    | Medium | Training and communication     |
| Technical skills   | Limited cloud/microservices skills | Medium    | High   | Training + hiring              |
| Data quality       | Duplicate employee records         | Low       | High   | Data cleansing/migration       |
| Change culture     | Moderate resistance                | Medium    | High   | Change-management program      |

> Exam memory

- Architecture Vision = `high-level capabilities + business value + desired direction.`
- And for Phase A, remember: `Vision → Value/KPIs → Risks/Mitigation → Statement of Architecture Work → Approval.`

## 6. Phase B: Business Architecture

The focus is to understand the Baseline Business Architecture, define the Target Business Architecture, and determine what must change to move from the current state to the desired state. It relates business elements to business goals and elements of other domains.

**Purpose** Develop the Target Business Architecture that supports the Architecture Vision and addresses the business drivers and objectives.

```bash
Baseline Business Architecture
          ↓
       Analysis
          ↓
Target Business Architecture
          ↓
      Gap Analysis
```

Baseline vs Target Business Architecture

|          | Baseline                        | Target                           |
| -------- | ------------------------------- | -------------------------------- |
| Meaning  | Current business state          | Desired future business state    |
| Focus    | How the business works today    | How the business should work     |
| Purpose  | Establish reference point       | Define future direction          |
| Example  | Manual employee onboarding      | Digital employee onboarding      |
| Used for | Understanding current situation | Defining required transformation |

Major Activities

| Step  | Activity                                          | Purpose                                                              |
| ----- | ------------------------------------------------- | -------------------------------------------------------------------- |
| **1** | Select reference models, viewpoints and tools     | Establish how the Business Architecture will be represented          |
| **2** | Develop Baseline Business Architecture            | Document the current business state                                  |
| **3** | Develop Target Business Architecture              | Define the desired future business state                             |
| **4** | Perform Gap Analysis                              | Identify differences between Baseline and Target                     |
| **5** | Define candidate roadmap components               | Identify major changes required                                      |
| **6** | Resolve impacts across the Architecture Landscape | Ensure business changes are consistent with other architecture areas |

Business Architecture Components

| Component               | Example                     |
| ----------------------- | --------------------------- |
| **Business Capability** | Employee Onboarding         |
| **Business Process**    | Onboard Employee            |
| **Business Function**   | HR Management               |
| **Organization**        | HR Department               |
| **Business Role**       | HR Officer                  |
| **Value Stream**        | Employee Lifecycle          |
| **Business Service**    | Employee Onboarding Service |

| Area               | Baseline         | Target               | Gap                     |
| ------------------ | ---------------- | -------------------- | ----------------------- |
| Onboarding         | Manual           | Automated            | Workflow capability     |
| Employee data      | Multiple sources | Centralized          | Data integration        |
| Account creation   | Manual           | Automated            | Provisioning capability |
| Communication      | Email            | Portal/notifications | Digital service         |
| Process monitoring | Limited          | Real-time            | Operational visibility  |

### Gap Analysis

A gap is the shortfall between the Baseline Architecture and the Target Architecture.

```bash
BASELINE                         TARGET
Current State                    Future State
     │                                │
     └────────── Compare ─────────────┘
                     │
                     ▼
                   GAPS
                     │
                     ▼
             What must change?
```

Suppose an organization currently performs employee onboarding manually.

**Baseline:**

- HR creates employee records manually
- Paper-based document collection
- Email-based approval
- No centralized onboarding status
- Manual account provisioning

**Target:**

- Digital onboarding portal
- Online document submission
- Automated approval workflow
- Centralized onboarding tracking
- Automated account provisioning

> The gaps are the differences between these two states.

| Area                | Baseline    | Target            | Gap                                       |
| ------------------- | ----------- | ----------------- | ----------------------------------------- |
| Employee onboarding | Manual      | Digital           | Digital onboarding capability             |
| Documents           | Paper/email | Online repository | Document management capability            |
| Approval            | Email       | Workflow          | Workflow automation                       |
| Status tracking     | Manual      | Centralized       | Onboarding tracking capability            |
| Account creation    | Manual      | Automated         | Identity/account provisioning integration |

> So the relationship is: `Baseline → Target → Gap Analysis → Change Requirements → Roadmap Components`

Baseline

```bash
Employee
   │
   ▼
HR Email
   │
   ▼
Manual HR Processing
   │
   ├── Documents
   ├── Approval
   ├── Employee Record
   └── Account Creation
```

Target

```bash
Employee
   │
   ▼
Digital Employee Portal
   │
   ▼
Workflow / Integration Layer
   │
   ├── HR Management
   ├── Document Management
   ├── Approval
   ├── Identity Management
   └── Employee Notification
```

Gap Register

| Gap ID  | Baseline                | Target                 | Gap / Required Change            |
| ------- | ----------------------- | ---------------------- | -------------------------------- |
| GAP-001 | Email-based onboarding  | Digital portal         | Employee self-service capability |
| GAP-002 | Manual approval         | Workflow               | Approval automation              |
| GAP-003 | Paper/email documents   | Digital documents      | Document management              |
| GAP-004 | Manual account creation | Automated provisioning | IAM integration                  |
| GAP-005 | No centralized tracking | Real-time status       | Onboarding tracking              |

Overall Approach

| Step  | Activity                                          | Main Question                                                           |
| ----- | ------------------------------------------------- | ----------------------------------------------------------------------- |
| **1** | Select reference models, viewpoints and tools     | How will we describe the Business Architecture?                         |
| **2** | Develop Baseline Business Architecture            | What does the business look like today?                                 |
| **3** | Develop Target Business Architecture              | What should the business look like in the future?                       |
| **4** | Perform Gap Analysis                              | What must change?                                                       |
| **5** | Define candidate roadmap components               | What changes/projects may be required?                                  |
| **6** | Resolve impacts across the Architecture Landscape | What impact does the Business Architecture have on other architectures? |

Step 1 — Select Reference Models, Viewpoints and Tools

Before creating the architecture, the architect determines how the business will be represented and analyzed. This includes selecting:

- Reference models
- Viewpoints
- Architecture tools

Why? Different stakeholders need different representations.

| Stakeholder          | Useful viewpoint                                 |
| -------------------- | ------------------------------------------------ |
| CEO                  | Business capabilities / value                    |
| HR Director          | HR processes and organizational responsibilities |
| Process Owner        | Business process                                 |
| Enterprise Architect | Cross-domain architecture                        |
| IT Manager           | Business-to-application relationship             |

> The important point is that the architecture representation should support stakeholder concerns.

Step 2 — Develop Baseline Business Architecture

Now document the current business state. You might capture:

- Business capabilities
- Business processes
- Business functions
- Organization structure
- Business roles
- Business services
- Value streams

```bash
Employee
   ↓
Email HR
   ↓
HR manually verifies documents
   ↓
Manager approval
   ↓
HR creates employee record
   ↓
IT manually creates accounts
```

Develop Target Business Architecture

Next define the future business state required to achieve the Architecture Vision. For your Digital Employee Platform.

```bash
Employee
   ↓
Digital Employee Portal
   ↓
Automated Workflow
   ├── Document Verification
   ├── Manager Approval
   ├── Employee Registration
   └── IT/IAM Provisioning
```

Step 4 — Perform Gap Analysis

```bash
Baseline Business Architecture
              │
              ▼
        GAP ANALYSIS
              ▲
              │
Target Business Architecture
```

| Baseline                | Target                 | Gap                           |
| ----------------------- | ---------------------- | ----------------------------- |
| Manual onboarding       | Digital onboarding     | Digital onboarding capability |
| Email approval          | Workflow approval      | Workflow capability           |
| Manual account creation | Automated provisioning | IAM integration capability    |
| Paper documents         | Digital documents      | Digital document capability   |

## 7. Phase C: Information Systems Architecture

It focuses on two architecture areas:

- Data Architecture
- Application Architecture

> The phase identifies gaps between the Baseline and Target Data & Application Architectures.

```bash
Phase B
Business Architecture
       │
       │ What does the business need?
       ▼
Phase C
Information Systems Architecture
       │
       ├── Data Architecture
       │
       └── Application Architecture
       │
       ▼
Phase D
Technology Architecture
```

The Two Parts of Phase C

| Architecture                 | Main Question                                                                                         |
| ---------------------------- | ----------------------------------------------------------------------------------------------------- |
| **Data Architecture**        | What information/data does the enterprise need?                                                       |
| **Application Architecture** | What applications/services are needed to manage and support that information and business capability? |

Steps & Approach

| Step  | Activity                                                     |
| ----- | ------------------------------------------------------------ |
| **1** | Select reference models, viewpoints and tools                |
| **2** | Develop Baseline Application & Data Architecture Description |
| **3** | Develop Target Application & Data Architecture Description   |
| **4** | Perform Gap Analysis                                         |
| **5** | Define candidate roadmap components                          |
| **6** | Continue to the remaining Phase C activities                 |

Perform Gap Analysis

| Area            | Baseline                | Target            | Gap                          |
| --------------- | ----------------------- | ----------------- | ---------------------------- |
| Employee Portal | None                    | Digital portal    | New application              |
| Integration     | Manual                  | API-based         | Integration capability       |
| Documents       | File/email              | Document service  | Document management          |
| Workflow        | Manual                  | Automated         | Workflow application/service |
| IAM             | Manual provisioning     | Automated         | IAM integration              |
| Employee data   | Multiple/manual sources | Controlled source | Data management improvement  |

> The slide specifically describes Phase C as identifying gaps between the Baseline and Target Data & Application Architectures.

Phase B vs Phase C

| Phase       | Architecture                     | Main Focus                                               |
| ----------- | -------------------------------- | -------------------------------------------------------- |
| **Phase B** | Business Architecture            | Business capabilities, processes, organization, services |
| **Phase C** | Information Systems Architecture | Data + Applications                                      |
| **Phase D** | Technology Architecture          | Technology infrastructure/platform                       |

**Data Architecture Artifacts**

- Data Entity/Data Component Catalog
- Application/Data Matrix
- Conceptual Data Diagram
- Data Dissemination Diagram
- Data Entity/Business Function Matrix
- Logical Data Diagram
- Data Security Diagram
- Data Migration Diagram
- Data Lifecycle Diagram

| Artifact                                 | What it represents                               |
| ---------------------------------------- | ------------------------------------------------ |
| **Data Entity/Data Component Catalog**   | Inventory of important data entities/components  |
| **Application/Data Matrix**              | Which applications use/manage which data         |
| **Conceptual Data Diagram**              | High-level relationships between data entities   |
| **Data Dissemination Diagram**           | How data is distributed/shared                   |
| **Data Entity/Business Function Matrix** | Relationship between business functions and data |
| **Logical Data Diagram**                 | More detailed logical structure of data          |
| **Data Security Diagram**                | Data security considerations                     |
| **Data Migration Diagram**               | Movement of data between systems                 |
| **Data Lifecycle Diagram**               | Data movement through its lifecycle              |

Data Entity/Data Component Catalog

| ID     | Data Entity       | Description                       |
| ------ | ----------------- | --------------------------------- |
| DE-001 | Employee          | Employee master information       |
| DE-002 | Department        | Organizational department         |
| DE-003 | Position          | Employee position                 |
| DE-004 | Employment        | Employment details                |
| DE-005 | Employee Document | Employee-related documents        |
| DE-006 | Onboarding        | Onboarding status and information |

Application/Data Matrix

| Data Entity       | Employee Portal | HR System |  IAM  |
| ----------------- | :-------------: | :-------: | :---: |
| Employee          |        X        |     X     |   X   |
| Department        |        X        |     X     |       |
| Employment        |                 |     X     |       |
| Employee Document |        X        |     X     |       |
| Onboarding        |        X        |     X     |       |
| Identity          |                 |           |   X   |

Data Entity / Business Function Matrix

| Data Entity       | Employee Onboarding | Payroll | Recruitment |
| ----------------- | :-----------------: | :-----: | :---------: |
| Employee          |          X          |    X    |      X      |
| Employment        |          X          |    X    |             |
| Payroll           |                     |    X    |             |
| Recruitment       |                     |         |      X      |
| Employee Document |          X          |         |      X      |

**Application Architecture Artifacts**

Application Portfolio Catalog

| ID       | Name                             | Category |
| -------- | -------------------------------- | -------- |
| L_APP_01 | Enterprise Resource Planning     | Platform |
| L_APP_02 | Customer Relationship Management | Platform |
| L_APP_03 | Data Warehouse                   | Platform |

Application / Organization Matrix

| Application | Sales |  HR   |
| ----------- | :---: | :---: |
| CRM         |   X   |       |
| ERP         |       |   X   |
| DWH         |   X   |   X   |
| DMS         |   X   |   X   |

Application Portfolio Catalog

| ID      | Application          | Purpose                        |
| ------- | -------------------- | ------------------------------ |
| APP-001 | Employee Portal      | Employee self-service          |
| APP-002 | HR System            | Employee management            |
| APP-003 | Workflow Service     | Process automation             |
| APP-004 | Document Management  | Employee documents             |
| APP-005 | IAM                  | Identity and access management |
| APP-006 | Notification Service | Email/SMS notifications        |

Application / Organization Matrix

| Application         |  HR   |  IT   | Finance | Employee |
| ------------------- | :---: | :---: | :-----: | :------: |
| Employee Portal     |   X   |   X   |         |    X     |
| HR System           |   X   |       |         |          |
| IAM                 |       |   X   |         |    X     |
| Payroll             |   X   |       |    X    |          |
| Document Management |   X   |   X   |         |    X     |

## 8. Phase D: Technology Architecture

Technology Architecture defines the technology environment required to support the target Business, Data, and Application Architectures. In simple terms:

- Business tells us what the enterprise needs.
- Data and Applications tell us what information and systems are required.
- Technology Architecture tells us what technology will run and support those systems.

**Primary purpose** Develop the Target Technology Architecture that enables the Architecture Vision and supports the Business, Data and Application Architectures.

**Objectives**

*Objective 1* — Develop the Target Technology Architecture
Define the future technology architecture needed to support the Architecture Vision, Business, Data, and Application Architectures.
In simple terms: What technology do we need in the future?

*Objective 2* — Identify Roadmap Components
Identify what needs to change to move from the Baseline Technology Architecture to the Target Technology Architecture.
In simple terms: What technology changes are required to get there?

Technology Stack/Portfolio Catalog

| ID      | Technology           | Category             | Purpose               |
| ------- | -------------------- | -------------------- | --------------------- |
| TEC-001 | Java 25              | Runtime              | Application runtime   |
| TEC-002 | Spring Boot          | Application Platform | Backend services      |
| TEC-003 | Oracle Database 26ai | Database             | Enterprise data       |
| TEC-004 | Nginx                | Web                  | Reverse proxy         |
| TEC-005 | Docker               | Container            | Application packaging |
| TEC-006 | Kubernetes           | Orchestration        | Container management  |

## 9. Phase E: Opportunities and Solutions

Phase E identifies the solution options and transition approach needed to move from the Baseline Architecture toward the Target Architecture. We now move from designing the architecture to deciding how to realize the Target Architecture. Your course outline for Phase E contains.

1. Interoperability & Risk Management
2. Architecture Roadmap
3. Implementation and Migration Plan

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
