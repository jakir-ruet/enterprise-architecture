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

*Example:*
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

Interoperability is the ability to share information and services.

| Type                       | Simple Meaning                                    | Key Question                            |
| -------------------------- | ------------------------------------------------- | --------------------------------------- |
| **Operational / Business** | Different parts of the enterprise work together   | How do business units collaborate?      |
| **Information**            | Information is shared between systems/people      | How is information shared?              |
| **Technical**              | Technical resources connect/share with each other | How do systems technically communicate? |

Maximize business benefit while minimizing business loss.

| Term                    | Meaning                                                                    |
| ----------------------- | -------------------------------------------------------------------------- |
| **Risk**                | Effect of uncertainty on objectives                                        |
| **Risk Trigger**        | Something inside or outside the transformation that may cause a risk event |
| **Initial Risk Level**  | Risk level before mitigation                                               |
| **Residual Risk Level** | Risk level after mitigation                                                |
| **Risk Mitigation**     | Actions taken to reduce the likelihood or impact of risk                   |

Initial Risk Assessment Matrix

| Effect       | Frequency  | Risk Level             |
| ------------ | ---------- | ---------------------- |
| Catastrophic | Frequent   | **Extremely High (E)** |
| Critical     | Likely     | **High (H)**           |
| Marginal     | Occasional | **Medium (M)**         |
| Negligible   | Seldom     | **Low (L)**            |
| —            | Unlikely   | **Low (L)**            |

| Risk                 | Type                |  Initial Level | Mitigation                  | Residual |
| -------------------- | ------------------- | -------------: | --------------------------- | -------: |
| API unavailable      | Technology/Business |           High | HA + monitoring             |   Medium |
| Employee data breach | Cyber               | Extremely High | Encryption + IAM + audit    |     High |
| Data mismatch        | Information         |           High | Validation + reconciliation |   Medium |
| Migration failure    | Business            |           High | Backup + rollback + testing |   Medium |

## 10. Phase F: Migration Planning

Phase F finalizes the Implementation and Migration Plan and prepares the enterprise for actual implementation.

Purpose - Phase E creates the draft transformation plan. Phase F makes it realistic, prioritized, resourced, and approved.

Objectives

| Objective                                                            | Original meaning                                                                           | Simple meaning                                                                         |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------- |
| **1. Finalize Architecture Roadmap & Implementation/Migration Plan** | Complete the roadmap and detailed migration plan                                           | **Finalize the roadmap and migration plan.**                                           |
| **2. Coordinate with enterprise change management**                  | Ensure migration aligns with the organization's overall change approach                    | **Make sure architecture migration fits the organization's overall change portfolio.** |
| **3. Ensure stakeholders understand value, cost & transitions**      | Make business value, work-package cost, and Transition Architectures clear to stakeholders | **Make sure stakeholders understand value, cost, and transition implications.**        |

Suppose a bank is moving from a legacy core banking platform to a cloud-based platform.

- Objective 1: Finalize the migration roadmap and project plan.
- Objective 2: Coordinate the migration with other major bank projects, such as CRM modernization and data-platform transformation.
- Objective 3: Make sure executives understand:
  - Value: faster digital services
  - Cost: migration and infrastructure investment
  - Transition: legacy and new systems may operate together temporarily.

> Phase F = Finalize the plan, align it with enterprise change, and make value/cost/transition clear to stakeholders.

Phase E vs Phase F

| Phase E                                     | Phase F                                   |
| ------------------------------------------- | ----------------------------------------- |
| Opportunities & Solutions                   | Migration Planning                        |
| Identifies work packages                    | Prioritizes migration projects            |
| Identifies Transition Architectures         | Finalizes transition/migration approach   |
| Creates roadmap                             | Finalizes roadmap                         |
| Initializes Implementation & Migration Plan | Completes Implementation & Migration Plan |
| More solution/transition focused            | More planning/prioritization focused      |

## 11. Phase G: Implementation Governance

Phase G — Implementation Governance ensures that implementation projects conform to the Target Architecture and provides architectural governance throughout implementation.

| Slide concept                  | Simple meaning                                               |
| ------------------------------ | ------------------------------------------------------------ |
| **Ensure compliance**          | Make sure the project follows the **Target Architecture**    |
| **Guide implementation teams** | Help the project team implement the architecture correctly   |
| **Manage priorities**          | Balance **success, value, effort, and risk**                 |
| **Architecture Governance**    | Control architecture decisions during implementation         |
| **Compliance Review**          | Check whether the implementation follows the architecture    |
| **Change Requests**            | Govern architecture changes that arise during implementation |
| **Post-implementation review** | Check the completed implementation                           |

## 12. Phase H: Architecture Change Management

Phase H makes sure the architecture continues to deliver business value and manages changes that occur after implementation. Phase H Steps

1. Establish value realization process
2. Deploy monitoring tools
3. Manage risks
4. Provide analysis for architecture change management
5. Develop change requirements to meet performance targets
6. Manage governance process
7. Activate the process to implement change

Phase G vs Phase H

| Phase G                          | Phase H                                        |
| -------------------------------- | ---------------------------------------------- |
| Implementation Governance        | Architecture Change Management                 |
| Focuses on implementation        | Focuses on changes after/around implementation |
| Checks architectural conformance | Manages architectural evolution                |
| Compliance reviews               | Change analysis                                |
| Architecture Contracts           | Change Requests                                |
| “Are we implementing correctly?” | “What needs to change now?”                    |

## 13. Requirements Management Phase

Requirements Management ensures that the right architecture requirements are identified, recorded, prioritized, monitored, changed, and made available to every relevant ADM phase. Your deck describes the Requirements Management Phase as the process that:

- Documents architecture requirements
- Evaluates requirements
- Distributes requirements
- Manages requirements throughout the ADM
- Maintains traceability from business strategy to requirements
- Maintains the complete set of requirements, including stakeholder preferences

**Purpose** The deck identifies five major purposes

| Purpose                                             | Meaning                                                              |
| --------------------------------------------------- | -------------------------------------------------------------------- |
| Manage architecture requirements throughout the ADM | Requirements are managed continuously                                |
| Operate the requirements management process         | Maintain the process                                                 |
| Ensure effective requirements management            | Keep requirements controlled                                         |
| Provide traceability                                | Connect requirements to vision, mission, business model and strategy |
| Maintain complete requirements                      | Include stakeholder preferences                                      |

> Easy memory: Manage → Operate → Ensure → Trace → Maintain

**Objectives** The deck gives three objectives:

- *Objective 1* Ensure that the Requirements Management process is sustained and operates for all ADM phases. In simple terms: Requirements Management must work throughout the ADM.
- *Objective 2* Manage architecture requirements identified during any execution of the ADM cycle or a phase. Meaning: A requirement can appear during any ADM phase.
- *Objective 3* Ensure that relevant architecture requirements are available for use by each phase as the phase is executed. Meaning: Each phase should have access to the requirements it needs.

Requirements Management — Core Flow

```bash
Business Goals
     ↓
Requirements
     ↓
Document
     ↓
Prioritize
     ↓
Baseline
     ↓
Monitor
     ↓
New/Changed Requirements
     ↓
Impact Assessment
     ↓
Update Requirements
     ↓
Feed relevant ADM phases
```

**Requirements Management Steps — 10-Step Summary**

| Step   | Requirement Management Activity         | Key Activities / Details                                                                                                                                    | Main Output / Result                                                                   |
| ------ | --------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| **1**  | **Identify Requirements**               | Analyze **business goals & scenarios, management information, value streams, and user experience**. Document the requirements.                              | **Architecture Requirements Specification** + **Architecture Requirements Repository** |
| **2**  | **Establish Baseline Requirements**     | Establish the baseline based on **approved stakeholder priorities**.                                                                                        | Approved **Baseline Requirements**                                                     |
| **3**  | **Monitor Baseline Requirements**       | Continuously monitor the baseline requirements to determine whether they remain valid.                                                                      | Validated / monitored baseline                                                         |
| **4**  | **Identify New & Changed Requirements** | Identify requirements that are **added, modified, or removed**. Re-assess requirement priorities.                                                           | Updated requirements and priorities                                                    |
| **5**  | **Analyze Changed Requirements**        | Identify changed requirements, record **new priorities and decisions**, resolve conflicts, and generate a **Requirements Impact Statement**.                | **Requirements Impact Statement (Version n)**                                          |
| **6**  | **Assess Impact**                       | Assess the impact of changed requirements on **previous and current ADM phases**. Decide whether to implement them in the **current or a later ADM cycle**. | **Requirements Impact Statement (Version n+1)**                                        |
| **7**  | **Implement Phase H Requirements**      | Implement requirements arising from **Phase H — Architecture Change Management**.                                                                           | Change-related requirements incorporated                                               |
| **8**  | **Update Requirements Repository**      | Update the **Architecture Requirements Repository**, including requirement changes and affected stakeholder views.                                          | Updated Requirements Repository                                                        |
| **9**  | **Implement Changes**                   | Implement the approved requirement changes.                                                                                                                 | Implemented changes                                                                    |
| **10** | **Conduct Gap Analysis**                | Conduct Gap Analysis for previous phases, identify **gap requirements**, record them, and revise the **Target Architecture** where necessary.               | Gap requirements + revised Target Architecture                                         |

Easy-to-Remember Flow

| Stage                   |    Steps | Purpose                                                       |
| ----------------------- | -------: | ------------------------------------------------------------- |
| **Establish**           |  **1–3** | Identify → Baseline → Monitor                                 |
| **Manage Changes**      |  **4–6** | Identify changes → Analyze → Assess impact                    |
| **Integrate**           |  **7–8** | Bring in Phase H requirements → Update repository             |
| **Implement & Improve** | **9–10** | Implement changes → Gap Analysis → Revise Target Architecture |

> Exam Memory: `Identify → Baseline → Monitor → Change → Analyze → Assess → Implement → Update → Implement → Gap Analysis`

**Requirements Impact Assessment** Requirements Impact Assessment assesses the current architecture requirements and specification to identify:

- What requirements have changed
- What changes should be made
- What implications those changes have for the architecture

The deck emphasizes that the approach considers new facts that may invalidate parts of the existing architecture.

Requirements Impact Assessment — Key Activities

| Activity                                 | What it means                                                                                  |
| ---------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **Assess changed requirements**          | Examine the new or modified requirements                                                       |
| **Assess impact on ADM phases**          | Determine which previous and current ADM phases are affected                                   |
| **Determine implementation cycle**       | Decide whether the requirement should be addressed in the **current** or a **later ADM cycle** |
| **Prioritize requirements**              | Consider stakeholder priorities and the results of the assessment                              |
| **Investigate implications**             | Determine what the requirement change means for the architecture                               |
| **Make recommendations**                 | Recommend how the requirements should be managed                                               |
| **Update Requirements Impact Statement** | Generate the appropriate version of the **Requirements Impact Statement**                      |
| **Update Repository**                    | Record changes and affected stakeholder views in the **Architecture Requirements Repository**  |

```bash
New / Changed Requirement
          ↓
   Assess the Impact
          ↓
 ┌────────┴─────────┐
 ↓                  ↓
Previous ADM      Current ADM
Phases            Phase(s)
 └────────┬─────────┘
          ↓
Determine when to implement
          ↓
Current ADM Cycle
       OR
Later ADM Cycle
          ↓
Requirements Impact Statement
          ↓
Update Requirements Repository
```

**Requirements Impact Statement** The Requirements Impact Statement captures the results of the impact assessment. According to the deck, its content includes:

| Content                             | Purpose                                                    |
| ----------------------------------- | ---------------------------------------------------------- |
| **Phases to be revisited**          | Identify ADM phases that may need to be reconsidered       |
| **Requirements prioritization**     | Identify who/what leads the prioritization and the results |
| **Investigation results**           | Record findings from the assessment                        |
| **Recommendations**                 | Recommend how the requirements should be managed           |
| **Specific requirement references** | Identify the affected requirements                         |
| **Stakeholder priority**            | Record the relevant stakeholder priority                   |
| **Repository reference numbers**    | Maintain traceability to the Requirements Repository       |

Suppose an organization is developing a new ERP architecture.

*Requirement:* ERP must support 5,000 users. During the architecture development, the business changes its strategy. New requirement, ERP must support 15,000 users and operations across multiple countries. Requirements Management detects this as a changed requirement.

Impact Assessment

| Question                            | Assessment                              |
| ----------------------------------- | --------------------------------------- |
| What changed?                       | User capacity and geographic scope      |
| Which architecture may be affected? | Business, Application, Data, Technology |
| Which ADM phases may need review?   | Potentially B, C and D                  |
| Current or later cycle?             | Decision based on impact and timing     |
| What must be documented?            | Requirements Impact Statement           |
| Where is it recorded?               | Architecture Requirements Repository    |

> - **Exam Memory**
> - Requirements Management = Continuously identify, manage, assess, trace and feed requirements throughout the ADM.
> - Requirements Impact Assessment = Determine how changed requirements affect the existing architecture and which ADM phases/cycles need to respond.

## 14. Applying the ADM

This module explains how the ADM is applied in practice rather than treating it as a rigid, linear sequence.

The three topics in the course deck are:

1. ADM Techniques & Iterations
2. Information Flow
3. Architecture Alternatives & Trade-off Method

### 14.1 ADM Techniques & Iterations

The TOGAF ADM is an iterative method. It is not a simple one-way waterfall process. ADM phases and their steps can be executed simultaneously, repeated, revisited, or skipped when the required information is already available or is not needed for a particular Architecture Project.

Iterations are driven by the information needs of the Architecture Project.

```text
Architecture Project
        |
        v
  Information Need
        |
        v
 Select relevant ADM path
        |
        +----------------------+
        |                      |
        v                      v
Concurrent phases       Return / repeat phases
        |                      |
        +----------+-----------+
                   v
            Required architecture
```

The deck identifies five iteration cycles:

| Iteration Cycle                           | Purpose                                                                          | Simple Meaning                   |
| ----------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------- |
| **1. Iteration through the entire ADM**   | Develop a comprehensive Architecture Landscape                                   | Run separate ADM cycles/projects |
| **2. Architecture Development Iteration** | Create architecture content and ensure the architecture is considered as a whole | Iterate within an ADM cycle      |
| **3. Architecture Capability Iteration**  | Create and evolve the Architecture Capability                                    | Improve the EA capability        |
| **4. Architecture Governance Iteration**  | Support governance of change activities                                          | Govern implementation/change     |
| **5. Transition Planning Iteration**      | Create change roadmaps for a defined architecture                                | Plan movement toward the target  |

#### Iteration through the Entire ADM

This iteration develops a comprehensive Enterprise Architecture Landscape.

- Projects can go through the entire ADM cycle.
- Each project/cycle is bounded by a **Request for Architecture Work**.
- Each project changes or extends the Architecture Landscape.
- Separate projects can operate their own ADM cycles concurrently (**parallel iteration**).
- One project can trigger another (**sequential iteration**) when further architecture work is required or when impacts are identified outside the original Request for Architecture Work.

```text
Project A ──→ Customer Platform Architecture
     |
     +────→ may trigger Project B
                    |
                    └──→ Detailed Data Architecture
```

#### Architecture Development Iteration

This is iteration within an ADM cycle. Projects may:

1. **Operate multiple ADM phases concurrently** to manage relationships between Business, Data, Application, and Technology architectures.
2. **Cycle between ADM phases** to cover multiple phases and converge on a detailed Target Architecture.
3. **Return to previous phases** to update work products, converge on an Architecture Roadmap or Implementation and Migration Plan, or respond to changed requirements.

| Pattern                      | Example                                                   |
| ---------------------------- | --------------------------------------------------------- |
| Multiple phases concurrently | B + C + D working together                                |
| Cycle between phases         | B → C → D → C → D                                         |
| Return to previous phase     | H change causes earlier architecture work to be revisited |

#### Architecture Capability Iteration

The ADM can also be used to create and evolve the Architecture Capability. This includes work around:

- Architecture approach
- Architecture principles
- Architecture scope
- Architecture vision
- Architecture governance
- EA organizational capability

#### Key Exam Point

> **The ADM is iterative. Multiple phases may be open concurrently, phases may be repeated, and a project does not necessarily need to execute every ADM phase.**

---

### 14.2 Information Flow

The deck explicitly states that the ADM is **not a linear waterfall process**.

The ADM is a logical method for developing knowledge and places key activity steps together so that relationships between activities and information flows can be understood.

The TOGAF crop-circle diagram is a stylized path showing essential information flow. It should **not** be interpreted as:

- a strict linear process model, or
- a representation of exact activity sequence.

#### Information Flow Between ADM Phases

In every ADM phase:

```text
Inputs
  |
  v
ADM Phase
  |
  v
Outputs
  |
  +──────────────→ Input to a later phase
  |
  +──────────────→ Updated / detailed later
```

Important principles:

- Every phase consumes inputs and generates outputs.
- The output of one phase can become the input to a later phase.
- Outputs can be updated or made more detailed in later phases.
- The work plan of an Enterprise Architecture team depends on the problem and development task.
- The **Request for Architecture Work** helps define the required work.
- Different requests can require different ADM paths and different outputs.

> **Exam Memory:** ADM phase outputs are information assets that can flow forward, be refined, or be revisited. The ADM is not a rigid waterfall sequence.

---

### 14.3 Building Block Specification Process

Building Blocks are used throughout the ADM to move from required architecture capabilities to implementable solutions.

The deck describes an evolutionary and iterative process based on:

- Required functions
- Imposed constraints
- Available products

```text
Business Goals & Objectives
          |
          v
Identify required ABBs
          |
          v
Architecture Definition
          |
          v
Refine selected ABBs
          |
          v
Solution Building Blocks
          |
          v
COTS / Custom Development
```

#### ABB vs SBB

| Building Block                        | Meaning                                                                                    | Main Question                    |
| ------------------------------------- | ------------------------------------------------------------------------------------------ | -------------------------------- |
| **ABB — Architecture Building Block** | Logical architecture capability/component required to meet business and architecture needs | **What capability is required?** |
| **SBB — Solution Building Block**     | Physical/implementation-specific component that realizes an ABB                            | **How will it be implemented?**  |

The deck highlights that **ABBs are defined in Phases A, B, C, and D and shaped as SBBs in Phase E**.

---

### 14.4 Architecture Alternatives & Trade-off Method

Sometimes multiple Target Architectures can satisfy the Architecture Vision, principles, and requirements.

A single architecture may not satisfy every stakeholder concern simultaneously.

Therefore, architects can:

1. Identify alternative Target Architectures.
2. Build understanding of different possibilities.
3. Identify trade-offs between alternatives.
4. Expose hidden agendas, principles, and requirements by presenting alternatives to stakeholders.
5. Select an alternative or combine features from multiple alternatives to create the proposed Target Architecture.

#### Why Consider Alternatives?

```text
Vision + Principles + Requirements
                |
                v
      Architecture Alternatives
          /          |          \
         /           |           \
        v            v            v
    Option A      Option B      Option C
        \            |            /
         \           |           /
          +------ Trade-offs ---+
                    |
                    v
          Proposed Target Architecture
```

#### Architecture Trade-Off Method

The technique described in the deck is:

| Step  | Activity                                                                                                         |
| ----- | ---------------------------------------------------------------------------------------------------------------- |
| **1** | Use the vision, principles, requirements, and other information to select criteria for different alternatives    |
| **2** | Define alternatives based on the criteria and build an understanding of each                                     |
| **3** | Select one alternative or combine features from multiple alternatives to create the proposed Target Architecture |

### Example

Suppose an organization needs a new enterprise integration platform.

| Criterion              | Alternative A | Alternative B | Alternative C |
| ---------------------- | ------------- | ------------- | ------------- |
| Cost                   | Low           | Medium        | High          |
| Scalability            | Medium        | High          | Very High     |
| Vendor dependency      | High          | Medium        | Low           |
| Implementation speed   | High          | Medium        | Low           |
| Operational complexity | Low           | Medium        | High          |

There may be no universally perfect option. The architect presents the alternatives and trade-offs to stakeholders so that the preferred Target Architecture can be selected based on business priorities and concerns.

> **Exam Memory:** Architecture alternatives exist because different architectures can satisfy the vision and requirements with different trade-offs. The architect helps stakeholders understand those trade-offs.

---

## 15. Content & Core Concepts

This module contains three topics:

1. Content Framework & Enterprise Metamodel
2. Enterprise Continuum
3. Architecture Repository

### 15.1 Content Framework & Enterprise Metamodel

The **Architecture Content Framework** provides a structured way to organize and describe architecture content. It supports consistency and completeness when producing architecture work products.

The Content Framework provides a structure for architecture content and acts as a companion to the ADM. It can be adapted to organizational needs.

```text
ADM
 |
 +-- Architecture Vision
 +-- Business Architecture
 +-- Information Systems Architecture
 +-- Technology Architecture
 +-- Opportunities & Solutions
 +-- Migration Planning
 +-- Implementation Governance
 +-- Change Management
        |
        v
Architecture Content
        |
        +-- Artifacts
        +-- Models
        +-- Work Products
```

#### Enterprise Metamodel

The **Enterprise Metamodel** defines entities within the enterprise and the relationships between them.

It provides a basis for identifying what needs to be represented in architecture models and how those elements relate to one another.

*Example:*

```text
Business Capability
       |
       v
Business Process
       |
       v
Application
       |
       v
Data
       |
       v
Technology
```

#### Content Framework vs Enterprise Metamodel

|               | Content Framework                                     | Enterprise Metamodel                                                       |
| ------------- | ----------------------------------------------------- | -------------------------------------------------------------------------- |
| Main question | What architecture content should we organize/produce? | What entities and relationships should we model?                           |
| Focus         | Architecture content and work products                | Enterprise entities and relationships                                      |
| Purpose       | Consistency and completeness of architecture content  | Consistency and completeness of architecture models                        |
| Example       | Catalogs, matrices, diagrams, deliverables            | Business capability, application, data, technology and their relationships |

> **Exam Memory:** Content Framework = structure the architecture content. Enterprise Metamodel = define the entities and relationships represented by the architecture.

---

### 15.2 Enterprise Continuum

The **Enterprise Continuum** is a classification mechanism for architecture and solution assets, with increasing detail and specialization.

It provides context for reuse and helps distinguish generic assets from increasingly organization-specific assets.

```text
Generic
  |
  v
Foundation
  |
  v
Common / Industry
  |
  v
Organization-Specific
```

The Enterprise Continuum consists of two complementary continuums:

- **Architecture Continuum** — classification of architecture assets.
- **Solution Continuum** — classification of solution assets.

|           | Architecture Continuum                | Solution Continuum                |
| --------- | ------------------------------------- | --------------------------------- |
| Focus     | Architecture components and artifacts | Solution components and artifacts |
| Purpose   | Classify architecture assets          | Classify solution assets          |
| Direction | Generic → specialized                 | Generic → specialized             |

The deck defines the **Solution Continuum** as a categorization mechanism with increasing detail and specialization for components and artifacts stored in the Solutions Landscape or Reference Library.

> **Exam Memory:** Enterprise Continuum = classification and organization of reusable architecture and solution assets.

---

### 15.3 Architecture Repository

The **Architecture Repository** provides a structured location for architecture assets and related information.

It can be implemented using architecture modeling tools, analytical tools, file/document repositories, or combinations of these.

A practical repository can contain:

| Repository Area                            | Purpose                                                                 |
| ------------------------------------------ | ----------------------------------------------------------------------- |
| **Architecture Metamodel / Framework**     | Organization-specific architecture structure                            |
| **Reference Library**                      | Reference models, guidelines, templates, patterns and reusable material |
| **Standards Library**                      | Standards and technical requirements                                    |
| **Architecture Landscape**                 | Baseline, Target, Transition and other architecture states              |
| **Solutions Landscape**                    | Solution building blocks and implementation solutions                   |
| **Architecture Requirements Repository**   | Authorized architecture requirements                                    |
| **Governance Repository / Governance Log** | Governance structures, parameters and governance records                |

```text
                 Architecture Repository
                         |
        +----------------+----------------+
        |                |                |
        v                v                v
 Reference Library   Standards Library  Governance
        |                |                |
        +----------------+----------------+
                         |
                         v
               Architecture Landscape
                         |
                         v
                 Solutions Landscape
                         |
                         v
            Requirements / Governance Data
```

> **Exam Memory:** Architecture Repository = structured storage and reuse of architecture assets, standards, requirements, solutions and governance information.

---

## 16. Architecture Governance & EA Capability

This module contains:

1. Corporate & EA Governance
2. Architecture Board & Capability

### 16.1 Corporate Governance

Governance is a system by which the current and future state are directed and controlled.

Corporate Governance concerns how an enterprise is directed and controlled and includes areas such as:

- Strategic direction
- Stakeholder rights and roles
- Performance objectives
- Accountability
- Transparency
- Responsible use of resources

### 16.2 Architecture Governance

**Architecture Governance** is a system by which Enterprise Architectures are directed and controlled.

It operates within a hierarchy of governance structures and may coexist with:

```text
Corporate Governance
        |
        v
Enterprise / EA Governance
        |
        v
IT Governance
        |
        v
Technology / Solution Governance
        |
        v
Project / Implementation Governance
```

Architecture Governance provides the discipline needed to ensure that architecture decisions, implementation activities, and changes remain aligned with approved architecture and organizational objectives.

### Governance Benefits

The deck highlights benefits including:

- Discipline
- Transparency
- Independency
- Accountability
- Responsibility
- Fairness

These principles support controlled and credible architecture decision-making.

---

### 16.3 Architecture Board

The **Architecture Board** is a cross-organizational body represented by key architecture stakeholders.

It is responsible for reviewing and maintaining architecture and overseeing implementation of the architecture strategy.

Typical responsibilities include:

- Improving architecture discipline and maturity.
- Ensuring consistency across sub-architectures.
- Enforcing Architecture Compliance.
- Establishing reuse targets.
- Ensuring EA remains flexible to business and technology needs.
- Providing escalation capability for out-of-bounds decisions.
- Monitoring Architecture Contracts.
- Resolving architecture ambiguity, issues, and conflicts.
- Providing advice and guidance.
- Granting dispensations where appropriate.
- Considering policy changes.

An important governance distinction is that decision rights concerning the Target Architecture remain with the appropriate stakeholders; the Architecture Board provides governance, review, recommendations, and escalation mechanisms.

> **Exam Memory:** Architecture Board = cross-organizational governance body for architecture oversight and compliance.

---

### 16.4 Architecture Capability

An **Architecture Capability** is an organizational capability that enables an enterprise to develop, use, and sustain architecture in order to govern change.

It includes:

- Organization
- Roles
- Responsibilities
- Skills
- Processes
- Governance
- Architecture content
- Architecture repository
- Supporting tools and practices

The TOGAF ADM can itself be used iteratively to develop and evolve the Architecture Capability.

```text
Architecture Capability
        |
        +-- Organization
        +-- People / Skills
        +-- Processes
        +-- Content Framework
        +-- Architecture Repository
        +-- Governance
        +-- Tools
        +-- Roadmap
```

### Architecture Capability Development

The deck shows that the capability can be developed through areas such as:

- Organization Model
- Process Model
- Architecture Content / Metamodel
- Architecture Repository
- EA Capability Roadmap

The roadmap can then transition into an Implementation and Migration Plan and be executed to build the desired EA Capability.

### Architecture Capability Benefits

The deck identifies benefits such as:

- Increased transparency of accountability and informed delegation of authority.
- Proactive risk and opportunity management.
- Protection of existing assets through reuse.
- Reuse of processes, concepts, and components across organizational units.
- Increased visibility supporting internal and external requirements.
- Internal value and shareholder value creation.

> **Exam Memory:** Architecture Governance = direct and control architecture. Architecture Board = governance body. Architecture Capability = organizational capability that enables EA and governance.

---

## 17. Exam Preparation & Definitions

This module contains:

1. Key Definitions
2. Exam Preparation & Time Management
3. Question Analysis & Answer Selection

### 17.1 Key Definitions

| Term                                  | Exam-Oriented Definition                                                                                                                                                          |
| ------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Architecture**                      | The fundamental concepts or properties of a system in its environment, embodied in its elements, relationships, and principles of design and evolution.                           |
| **Architecture Domain**               | A representation of a specific area of architecture, such as Business, Data, Application, or Technology.                                                                          |
| **Architecture Framework**            | A conceptual structure used to develop, use, and sustain an architecture.                                                                                                         |
| **Architecture Governance**           | A system by which Enterprise Architectures are directed and controlled.                                                                                                           |
| **ADM**                               | The TOGAF Architecture Development Method used to develop and use Enterprise Architecture.                                                                                        |
| **Architecture Building Block (ABB)** | A logical architecture component that describes what capability is required.                                                                                                      |
| **Solution Building Block (SBB)**     | An implementation-specific component that realizes one or more ABBs.                                                                                                              |
| **Architecture View**                 | A representation of a system from the perspective of related concerns.                                                                                                            |
| **Architecture Viewpoint**            | A specification of the conventions for constructing and using an architecture view.                                                                                               |
| **Stakeholder**                       | An individual, team, organization, or class thereof having an interest in a system.                                                                                               |
| **Requirement**                       | A statement of need that must be met by an architecture or solution.                                                                                                              |
| **Solution Continuum**                | A categorization mechanism for solution components and artifacts with increasing detail and specialization.                                                                       |
| **Standards Library**                 | A library of standards used to define services and components of an Organization-Specific Architecture.                                                                           |
| **Strategic Architecture**            | A summary formal description of the enterprise providing an organizing framework for operational and change activity and an executive-level long-term view for direction setting. |
| **Technology Architecture**           | A description of the structure and interaction of technology services and technology components.                                                                                  |
| **Transition Architecture**           | A formal description of one state of the architecture at an architecturally significant point in time.                                                                            |
| **Target Architecture**               | The description of a future state of the architecture being developed for an organization.                                                                                        |
| **Value Stream**                      | An end-to-end collection of activities that create an overall result for a customer, stakeholder, or end user.                                                                    |
| **Viewpoint Library**                 | A collection of specifications of architecture viewpoints contained in the Reference Library portion of the Architecture Repository.                                              |
| **Work Package**                      | A set of actions identified to achieve one or more objectives for the business.                                                                                                   |

These definitions are drawn from the definition material in the course deck. fileciteturn32file6

---

### 17.2 TOGAF Foundation Exam Preparation

The deck identifies the TOGAF Enterprise Architecture Part 1 Foundation exam as **OGEA-101** and describes the exam as:

| Item                                                   | Format                 |
| ------------------------------------------------------ | ---------------------- |
| Questions                                              | **40**                 |
| Question type                                          | **Single choice**      |
| Time                                                   | **60 minutes**         |
| Additional time stated in deck for non-native speakers | **30 minutes**         |
| Book                                                   | **Closed book**        |
| Pass mark                                              | **60% — 24 out of 40** |

The deck recommends three preparation activities:

1. **Study the content** — especially the ADM, its phases, techniques, and deliverables.
2. **Complete exam questions** — become familiar with the structure and characteristics of the exam.
3. **Test under real conditions** — simulate 40 questions in 60 minutes.

It also recommends testing the exam infrastructure and ensuring a quiet environment and redundant internet connection for a proctored exam.

---

### 17.3 Time Management

The deck recommends maintaining a constant pace.

For a 60-minute / 40-question exam:

```text
60 minutes / 40 questions
        |
        v
~90 seconds per question
```

Recommended approach:

- Move quickly through questions you understand.
- Skip difficult questions temporarily rather than getting stuck.
- Return to uncertain questions later.
- Use remaining time for a quality check.
- Review the questions where you have the most doubt.

> **Important:** The deck states that wrong answers do not receive negative points, so answer every question.

---

### 17.4 Question Analysis

Read every question and every answer option carefully.

Look for key TOGAF terms such as:

- Stakeholder
- Concern
- Viewpoint
- Governance
- Architecture Vision
- Requirements
- Building Block
- Roadmap
- Compliance
- Migration
- Architecture Capability

A useful process is:

```text
Read the Question
       |
       v
Identify Key Terms
       |
       v
Identify ADM Phase / Concept
       |
       v
Eliminate Distractors
       |
       v
Compare Similar Answers
       |
       v
Select the TOGAF-Aligned Answer
```

#### ADM Phase Recognition

| Question Clue               | Likely Focus            |
| --------------------------- | ----------------------- |
| Architecture Capability     | Preliminary Phase       |
| Vision / business value     | Phase A                 |
| Business Architecture       | Phase B                 |
| Data / Application          | Phase C                 |
| Technology Architecture     | Phase D                 |
| Opportunities / Solutions   | Phase E                 |
| Migration Planning          | Phase F                 |
| Implementation / Compliance | Phase G                 |
| Architecture Change         | Phase H                 |
| Continuous requirements     | Requirements Management |

---

### 17.5 Answer Selection

The deck recommends:

1. **Stick to the TOGAF spirit** — choose the answer most closely matching TOGAF concepts, phases, deliverables, and techniques.
2. **Sort out the distractor** — eliminate options that are clearly unrelated to TOGAF.
3. **Look for similar answers** — when two options appear plausible, carefully compare their wording and alignment with TOGAF.
4. **Always answer** — there is no benefit to leaving a question unanswered.

> **Exam Strategy:** Do not answer according to what would merely be a good IT practice. Answer according to the TOGAF concept described in the question.

---

## 18. Practice Test

The course deck includes a **TOGAF Enterprise Architecture Part 1 Sample Exam** with **40 questions, answers, and explanations**.

The practice test should be used as a realistic exam simulation rather than simply as a reading exercise.

### Practice-Test Rules

```text
40 Questions
     |
     v
60 Minutes
     |
     v
Single Choice
     |
     v
Closed Book
     |
     v
Target: 24/40 or higher
```

### Recommended Practice Process

**Round 1 — Full Simulation**

- Answer all 40 questions.
- Use a 60-minute timer.
- Do not consult notes.
- Mark uncertain questions.

**Round 2 — Review**

For every incorrect answer:

1. Identify the TOGAF concept.
2. Identify the relevant ADM phase.
3. Determine why the selected answer was wrong.
4. Determine why the correct answer is better.
5. Record the knowledge gap.

**Round 3 — Weak-Area Revision**

Group mistakes into categories:

| Category        | Examples                                         |
| --------------- | ------------------------------------------------ |
| EA Fundamentals | Architecture, domains, stakeholders, concerns    |
| ADM             | Phases, iteration, information flow              |
| Content         | Artifacts, deliverables, building blocks         |
| Architecture    | Business, Data, Application, Technology          |
| Migration       | Roadmap, work packages, Transition Architectures |
| Requirements    | Requirements Management, Impact Assessment       |
| Governance      | Architecture Board, Contracts, Compliance        |
| Repository      | Enterprise Continuum, Architecture Repository    |
| Definitions     | Foundation terminology                           |

### Practice-Test Performance Record

| Attempt | Correct | Wrong | Score | Target Met? | Weak Areas |
| ------: | ------: | ----: | ----: | :---------: | ---------- |
|       1 |         |       |       |             |            |
|       2 |         |       |       |             |            |
|       3 |         |       |       |             |            |
|       4 |         |       |       |             |            |
|       5 |         |       |       |             |            |

### Target

> **Minimum passing benchmark from the course deck: 24/40 (60%).**

For preparation, a stronger target is to achieve a stable score above the passing threshold across several timed practice attempts before sitting the actual exam.

> The deck establishes that the practice test contains 40 questions, answers, and explanations. The individual question text is intentionally not reproduced here unless it is directly extracted from the supplied deck; this README therefore does not invent questions and incorrectly attribute them to the course material.

---

## 19. Wrap-up

Congratulations — you have completed the **TOGAF Enterprise Architecture Foundation** study roadmap.

The course has taken you from Enterprise Architecture fundamentals through the ADM, architecture domains, migration, governance, content management, requirements, exam preparation, and practice testing.

### Complete Learning Journey

```text
01  Introduction to Enterprise Architecture
        |
02  Architecture Domains
        |
03  Architecture Development Method (ADM)
        |
04  Preliminary Phase
        |
05  Phase A — Architecture Vision
        |
06  Phase B — Business Architecture
        |
07  Phase C — Information Systems Architecture
        |
08  Phase D — Technology Architecture
        |
09  Phase E — Opportunities & Solutions
        |
10  Phase F — Migration Planning
        |
11  Phase G — Implementation Governance
        |
12  Phase H — Architecture Change Management
        |
13  Requirements Management
        |
14  Applying the ADM
        |
15  Content & Core Concepts
        |
16  Architecture Governance & EA Capability
        |
17  Exam Preparation & Definitions
        |
18  Practice Test
        |
19  Wrap-up
```

### Final TOGAF Mental Model

```text
                         ENTERPRISE ARCHITECTURE
                                  |
                                  v
                         Architecture Capability
                                  |
                                  v
                            PRELIMINARY
                                  |
                                  v
                         A — Architecture Vision
                                  |
                    +-------------+-------------+
                    |             |             |
                    v             v             v
                    B             C             D
                 Business     Data/App      Technology
                    +-------------+-------------+
                                  |
                                  v
                       E — Opportunities & Solutions
                                  |
                                  v
                       F — Migration Planning
                                  |
                                  v
                       G — Implementation Governance
                                  |
                                  v
                       H — Architecture Change Management
                                  |
                                  +------> New ADM Cycle

                 Requirements Management
                         <--- Continuous --->

                 Governance
                     |
                     v
               Architecture Board

                 Architecture Content
                     |
                     v
          Content Framework + Metamodel
                     |
                     v
              Enterprise Continuum
                     |
                     v
              Architecture Repository
```

### Five Core Memory Rules

| Concept                     | Remember                                                                                                |
| --------------------------- | ------------------------------------------------------------------------------------------------------- |
| **Architecture Domains**    | **WHAT** — Business, Data, Application, Technology                                                      |
| **ADM**                     | **HOW** — develop and manage architecture                                                               |
| **Requirements Management** | **CONTINUOUS** — requirements flow throughout the ADM                                                   |
| **Architecture Governance** | **CONTROL** — direct and control architecture                                                           |
| **Architecture Repository** | **STORE & REUSE** — architecture assets, requirements, standards, solutions, and governance information |

### ADM One-Line Memory

```text
Prepare
  ↓
Vision
  ↓
Business → Information Systems → Technology
  ↓
Opportunities & Solutions
  ↓
Migration Planning
  ↓
Implementation Governance
  ↓
Change Management
  ↺
```

### Final Exam Checklist

Before taking the Foundation exam, make sure you can explain without notes:

- [ ] Enterprise Architecture definition, purpose, and benefits
- [ ] Four Architecture Domains
- [ ] Baseline, Target, Transition, Candidate, and Resting Architecture States
- [ ] ADM phases and their purposes
- [ ] Preliminary Phase and Architecture Capability
- [ ] Architecture Principles
- [ ] Phase A and Architecture Vision
- [ ] Phase B Business Architecture
- [ ] Phase C Data and Application Architecture
- [ ] Phase D Technology Architecture
- [ ] Phase E Opportunities and Solutions
- [ ] Phase F Migration Planning
- [ ] Phase G Implementation Governance
- [ ] Phase H Architecture Change Management
- [ ] Requirements Management and Requirements Impact Assessment
- [ ] ADM iteration and information flow
- [ ] Architecture Building Blocks vs Solution Building Blocks
- [ ] Architecture alternatives and trade-offs
- [ ] Content Framework and Enterprise Metamodel
- [ ] Enterprise Continuum
- [ ] Architecture Repository
- [ ] Corporate and Architecture Governance
- [ ] Architecture Board
- [ ] Architecture Capability
- [ ] Key TOGAF definitions
- [ ] Exam time management
- [ ] Question analysis and answer selection
- [ ] 40-question timed practice test

### Final Preparation Rule

> **Know the TOGAF terminology, understand the ADM logic, recognize the phase from the question, eliminate distractors, and select the answer that most closely matches the TOGAF Standard.**

### Course Completion

The course deck closes with congratulations and good wishes for the **TOGAF Enterprise Architecture Part 1 Exam (Foundation)**.

> **Good luck with your TOGAF Enterprise Architecture Part 1 Foundation exam.**

---

## Recommended Next Step

After completing this roadmap, use the supplied 40-question practice test as a timed mock exam. Record your score and every incorrect answer. Then revise the corresponding module before attempting the next mock exam.

```text
Study
  ↓
Practice Test
  ↓
Analyze Mistakes
  ↓
Identify Weak Areas
  ↓
Revise
  ↓
Retest
  ↓
Repeat Until Consistent
```
