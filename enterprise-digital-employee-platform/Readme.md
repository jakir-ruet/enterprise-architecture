### Complete architecture lifecycle

```bash
Business
   ↓
Data
   ↓
Application
   ↓
Technology
   ↓
Security
   ↓
Integration
   ↓
Migration
   ↓
Implementation
   ↓
Governance
```

### The fictional enterprise

**For our exercise, assume:** ABC Enterprise is a large organization with approximately 5,000 employees operating across multiple business units. It currently has several independent systems.

```bash
                         ABC ENTERPRISE
                               │
       ┌───────────────────────┼───────────────────────┐
       │                       │                       │
      HR                    Finance                    IT
       │                       │                       │
       ▼                       ▼                       ▼
   HR System              Payroll System          Identity System
       │                       │                       │
       └───────────────┬───────┴───────────────────────┘
                       │
                 Other Systems
                       │
              ┌────────┴────────┐
              │                 │
          Attendance          Leave
           System             System
```

> The systems work, but they were developed independently over time.

#### Current business problems (ABC Enterprise has the following problems.)

**Problem 1** — Fragmented employee experience. Employees need to use multiple systems.

```bash
Employee
   │
   ├── HR System
   ├── Leave System
   ├── Attendance System
   ├── Payroll System
   └── Document System
```

> There is no unified employee portal.

**Problem 2** — Duplicate data. Employee information exists in multiple systems.

```bash
HR Database
    │
    ├── Employee Name
    ├── Email
    ├── Department
    └── Position

Attendance Database
    │
    ├── Employee Name
    ├── Employee ID
    └── Department

Payroll Database
    │
    ├── Employee Name
    ├── Employee ID
    └── Salary
```

> This creates data consistency problems.

**Problem 3** — Point-to-point integration. Systems communicate directly with each other.

```bash
HR ─────────► Payroll
 │              │
 ├──────────► Attendance
 │              │
 └──────────► Leave
```

> As the number of systems grows, integration becomes increasingly difficult.

**Problem 4** — Manual processes. Some employee processes still rely on:

- Email
- Excel
- Manual approvals
- Manual data entry
- Manual reporting

**Problem 5** — Limited observability. Operations teams don't have a unified view of:

- application health
- API performance
- database performance
- integration failures
- business transactions

**Problem 6** — Security inconsistency. Different applications have different:

- authentication mechanisms
- authorization models
- audit mechanisms
- password policies

### Business vision

**ABC Enterprise wants to build:** A secure, integrated, scalable digital employee platform providing a single access point to employee services and enabling standardized enterprise integration and data governance.

**The target experience:**

```bash
						EMPLOYEE
							│
							▼
				┌─────────────────┐
				│ Employee Portal │
				└────────┬────────┘
							│
							▼
				┌──────────────┐
				│ API Gateway  │
				└──────┬───────┘
						│
		┌─────────────┼─────────────┐
		▼             ▼             ▼
Employee        Leave       Attendance
Service        Service       Service
		│             │             │
		└─────────────┼─────────────┘
						│
				Integration Layer
						│
		┌─────────────┼─────────────┐
		▼             ▼             ▼
	HR           Payroll        IAM
```

### Business capabilities

Before choosing applications, we identify the business capabilities.

```bash
Employee Management
│
├── Employee Master Data
├── Organization Management
├── Position Management
└── Employee Lifecycle

Leave Management
│
├── Leave Request
├── Leave Approval
├── Leave Balance
└── Leave Reporting

Attendance Management
│
├── Attendance Capture
├── Shift Management
└── Attendance Reporting

Payroll Integration
│
├── Payroll Data Exchange
├── Payroll Status
└── Payroll Reporting

Identity & Access
│
├── Authentication
├── Authorization
├── SSO
└── Access Governance

Analytics
│
├── Operational Reporting
├── Management Dashboard
└── Workforce Analytics
```

> Important architecture lesson:

- We are not saying: "Let's create six microservices."
- We're saying: "These are the business capabilities the enterprise needs."

The application architecture will come later.

### Project objectives - The architecture must support these objectives

| #   | Objective                                         |
| --- | ------------------------------------------------- |
| 1   | Provide a unified employee experience             |
| 2   | Establish a trusted employee master data model    |
| 3   | Reduce manual HR processes                        |
| 4   | Standardize enterprise integration                |
| 5   | Improve security and access control               |
| 6   | Improve operational visibility                    |
| 7   | Enable scalable digital services                  |
| 8   | Establish API-first integration                   |
| 9   | Enable event-driven integration where appropriate |
| 10  | Establish architecture governance                 |

### Initial scope

```bash
✓ Employee Management
✓ Employee Portal
✓ Leave Management
✓ Attendance Integration
✓ Payroll Integration
✓ Identity / SSO
✓ API Management
✓ Event Integration
✓ Reporting
✓ Audit
✓ Security
✓ Observability
```

### Out of scope initially

```bash
✗ Recruitment
✗ Performance Management
✗ Learning Management
✗ Full ERP replacement
✗ Full Payroll replacement
```

> This gives us a manageable architecture boundary.

### Technology constraints

#### Application platform

```bash
Java 25
    │
    ▼
Spring Boot
    │
    ├── Spring Web
    ├── Spring Security
    └── Spring JDBC
```

#### Database

```bash
Spring JDBC
      │
      ▼
Oracle JDBC Driver
      │
      ▼
Oracle Database 26ai
```

#### Integration

```bash
REST APIs
     +
Kafka Events
```

#### Platform

```bash
Docker
   ↓
Kubernetes
   ↓
AWS / Hybrid Infrastructure
```

#### DevOps

```bash
Git
 ↓
Maven
 ↓
CI
 ↓
Security Scanning
 ↓
Docker
 ↓
Kubernetes
```

### Important architectural constraint - We will not use JPA/Hibernate

```bash
Controller
    ↓
Application Service
    ↓
Repository
    ↓
Spring JDBC
    ↓
Oracle JDBC Driver
    ↓
Oracle 26ai
```

### Stakeholders

| Stakeholder          | Primary concern        |
| -------------------- | ---------------------- |
| CEO                  | Business value         |
| CIO/CTO              | Technology strategy    |
| HR Director          | Employee processes     |
| Finance Director     | Payroll                |
| IT Manager           | Operations             |
| Enterprise Architect | Architecture integrity |
| Solution Architect   | Solution design        |
| Data Architect       | Data governance        |
| Security Architect   | Security               |
| DevOps Team          | Deployment             |
| Employees            | User experience        |
| Managers             | Approvals/reporting    |

### Business drivers - The architecture is driven by:

```bash
Digital Transformation
        │
        ├── Employee Experience
        ├── Operational Efficiency
        ├── Data Quality
        ├── Integration Modernization
        ├── Security
        ├── Compliance
        ├── Scalability
        ├── Automation
        └── Analytics
```

### Architecture principles - We'll adopt these as our initial principles

1. **P01 — Business-driven architecture** - Technology must support measurable business outcomes.
2. **P02 — API-first** - Enterprise capabilities should be exposed through well-defined APIs where appropriate.
3. **P03 — Security by design** - Security is an architectural concern from the beginning.
4. **P04 — Separation of concerns** - Presentation, business logic, persistence, integration and infrastructure responsibilities remain appropriately separated.
5. **P05 — Observability by design** - Critical services provide logs, metrics, traces and audit events.
6. **P06 — Automation first** - Build, test, deployment and infrastructure processes should be automated.
7. **P07 — Reuse before duplication** - Existing approved enterprise capabilities should be reused.
8. **P08 — Data ownership** - Critical data must have clear ownership and stewardship.
9. **P09 — Resilience proportional to business criticality** - Availability, backup and DR requirements must reflect business importance.
10. **P10 — Architecture decisions are documented** - Significant architecture decisions require traceable ADRs.

### Success criteria - For this hands-on project, we'll use the following initial target values

| KPI                            |  Target |
| ------------------------------ | ------: |
| Critical platform availability | ≥ 99.9% |
| Employee self-service adoption |   ≥ 80% |
| Manual HR processing reduction |   ≥ 50% |
| Critical API observability     |    100% |
| Critical transactions audited  |    100% |
| CI/CD deployment automation    |    100% |
| Critical APIs documented       |    100% |
| Centralized authentication     |    100% |

### TOGAF hands-on project

```bash
┌─────────────────────────────────────┐
│       TOGAF hands-on project        │
├─────────────────────────────────────┤
│ Step 0  Project Definition      ✓   │
│ Step 1  Preliminary Phase       →   │
│ Step 2  Architecture Vision         │
│ Step 3  Business Architecture       │
│ Step 4  Data Architecture           │
│ Step 5  Application Architecture    │
│ Step 6  Technology Architecture     │
│ Step 7  Opportunities & Solutions   │
│ Step 8  Migration Planning          │
│ Step 9  Implementation Governance   │
│ Step 10 Architecture Change         │
└─────────────────────────────────────┘
```

---

### Step 1 — Preliminary Phase: Establish the Architecture Capability

#### Preliminary Phase objective

For our project: Establish an architecture capability that defines governance, principles, standards, roles, decision-making, compliance, and the architecture repository. Our flow is:

```bash
						PRELIMINARY PHASE
								│
		┌───────────────────┼───────────────────┐
		▼                   ▼                   ▼
Governance          Principles          Standards
		│                   │                   │
		└───────────────────┼───────────────────┘
								▼
							Architecture
							Repository
								│
								▼
						Decision Process
								│
								▼
						Compliance / Review
```

#### Architecture Organization - We'll establish the following structure

```bash
								CIO / CTO
									│
									▼
					Architecture Review Board
									│
				┌──────────────┼──────────────┐
				│              │              │
				▼              ▼              ▼
	Enterprise        Security          Data
		Architect        Architect        Architect
				│
				▼
		Solution Architect
				│
	┌──────┼──────┬─────────────┐
	▼      ▼      ▼             ▼
Application DevOps Infrastructure Integration
Architect   Lead     Architect      Architect
```

**Your role in the project** - You are the: **Enterprise Architect** - You are responsible for:

- Architecture vision
- Architecture principles
- Architecture decisions
- Cross-domain alignment
- Architecture governance
- Target architecture
- Technology standards
- Architecture roadmap

#### Architecture Review Board - We'll create an Architecture Review Board (ARB)

| Role                  | Responsibility           |
| --------------------- | ------------------------ |
| CIO/CTO               | Executive sponsorship    |
| Enterprise Architect  | Architecture authority   |
| Solution Architect    | Solution design          |
| Application Architect | Application architecture |
| Data Architect        | Data architecture        |
| Security Architect    | Security                 |
| Technology Architect  | Infrastructure/platform  |
| DevOps Lead           | CI/CD and automation     |
| Business Owner        | Business alignment       |

#### Architecture Domains

```bash
					Enterprise Architecture
								│
	┌──────────┬──────────┼──────────┬──────────┐
	│          │          │          │          │
Business     Data    Application Technology Security
	│          │          │          │          │
	└──────────┴──────────┴──────────┴──────────┘
								│
						Integration
```

> We'll also treat Integration as a cross-cutting architecture concern.

#### Architecture Principles

| ID         | Domain      | Principle                        | Description                                                                                                                           | Rationale / Implementation Guidance                                                                                                |
| ---------- | ----------- | -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| **BP-001** | Business    | **Business-Driven Architecture** | Architecture decisions must support measurable business outcomes.                                                                     | Technology exists to enable business capabilities and strategic objectives.                                                        |
| **BP-002** | Business    | **Capability Alignment**         | Applications and technologies must support identified business capabilities.                                                          | **Business Capability → Business Service → Application Capability → Technology**                                                   |
| **BP-003** | Business    | **Reuse Before Duplication**     | Existing approved enterprise capabilities should be reused before creating new ones.                                                  | Reduces cost, complexity, duplication, and long-term maintenance.                                                                  |
| **DP-001** | Data        | **Data Ownership**               | Every critical business data domain must have an accountable owner.                                                                   | Example: **Employee Master Data → HR**. Ownership ensures accountability for quality, access, lifecycle, and governance.           |
| **DP-002** | Data        | **Data Integrity**               | Critical enterprise data must maintain consistency, accuracy, referential integrity, and transactional integrity.                     | Oracle Database 26ai will be the primary transactional database for the platform.                                                  |
| **DP-003** | Data        | **Data Security**                | Sensitive employee information must be protected through authorization, encryption, auditing, least privilege, and controlled access. | Protects confidentiality, integrity, and regulatory compliance of enterprise data.                                                 |
| **AP-001** | Application | **API-First**                    | Application capabilities that need to be consumed by other systems should expose well-defined APIs.                                   | Default approach: **REST → JSON → OpenAPI**. APIs should be versioned, secured, documented, and reusable.                          |
| **AP-002** | Application | **Separation of Concerns**       | Presentation, application/business logic, persistence, and integration responsibilities should remain appropriately separated.        | Target application structure: **Controller → Application Service → Repository → JDBC → Oracle 26ai**.                              |
| **AP-003** | Application | **JDBC-Based Data Access**       | The platform will use JDBC/Spring JDBC rather than an ORM framework.                                                                  | **JPA  / Hibernate  / JDBC ✓ / Spring JDBC ✓**. Provides explicit SQL and direct control over Oracle database interactions.        |
| **TP-001** | Technology  | **Automation First**             | Repeatable build, test, security scanning, packaging, and deployment processes should be automated.                                   | Target pipeline: **Code → Build → Test → Security Scan → Container → Deploy**.                                                     |
| **TP-002** | Technology  | **Observability by Design**      | Critical services must provide operational visibility through logs, metrics, health checks, tracing, and audit events.                | Spring Boot services should be observable from development through production.                                                     |
| **TP-003** | Technology  | **Infrastructure as Code**       | Infrastructure should be defined and provisioned through version-controlled, repeatable automation.                                   | Target approach: **Terraform → AWS/Infrastructure → Kubernetes → Applications**.                                                   |
| **SP-001** | Security    | **Security by Design**           | Security requirements must be considered during architecture and design rather than added after implementation.                       | Authentication, authorization, encryption, secrets management, auditability, and threat controls are architectural concerns.       |
| **SP-002** | Security    | **Least Privilege**              | Users, applications, services, and administrators should receive only the permissions required to perform their responsibilities.     | Minimize the potential impact of compromised accounts or services.                                                                 |
| **SP-003** | Security    | **Centralized Identity**         | Authentication and identity management should be centralized rather than independently implemented by each application.               | Target: **User → Keycloak/IdP → OIDC/OAuth2 → Spring Boot APIs**.                                                                  |
| **SP-004** | Security    | **Auditability**                 | Security-sensitive and business-critical activities must be auditable.                                                                | Audit events should capture sufficient information to support security investigation, compliance, and operational troubleshooting. |

#### Technology Standards

| Area                 | Standard                  |
| -------------------- | ------------------------- |
| Programming language | Java 25                   |
| Framework            | Spring Boot               |
| Data access          | Spring JDBC / JDBC        |
| ORM                  | None                      |
| Database             | Oracle Database 26ai      |
| Database driver      | Oracle JDBC               |
| API                  | REST                      |
| API format           | JSON                      |
| API specification    | OpenAPI                   |
| Authentication       | OAuth 2.0 / OIDC          |
| Identity             | Keycloak                  |
| Messaging            | Apache Kafka              |
| Build                | Maven                     |
| Source control       | Git                       |
| Container            | Docker                    |
| Orchestration        | Kubernetes                |
| IaC                  | Terraform                 |
| Configuration        | Ansible where appropriate |
| Metrics              | Prometheus                |
| Visualization        | Grafana                   |

> These are our initial standards, not immutable rules. Later architecture decisions can modify them through governance.
