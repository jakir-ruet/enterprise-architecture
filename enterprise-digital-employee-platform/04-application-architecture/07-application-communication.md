# Application Communication Diagram

## Target Communication View

```mermaid
flowchart LR
    USER[Employee / Manager / HR]
    PORTAL[Digital Employee Portal]
    IAM[IAM / SSO]
    API[API Gateway]
    HR[HR Core]
    LEAVE[Leave & Attendance]
    PERF[Performance]
    REC[Recruitment]
    PAY[Payroll]
    BUS[Event / Message Bus]
    DATA[Data Platform]
    ANA[Analytics]

    USER --> PORTAL
    PORTAL --> IAM
    PORTAL --> API
    API --> HR
    API --> LEAVE
    API --> PERF
    API --> REC
    API --> PAY
    HR --> BUS
    LEAVE --> BUS
    PERF --> BUS
    REC --> BUS
    PAY --> BUS
    BUS --> DATA
    DATA --> ANA
```

## Communication Rules

- User-facing applications authenticate through central IAM.
- Business applications expose governed APIs for synchronous interactions.
- Domain events are used where asynchronous decoupling is beneficial.
- Sensitive data must use authenticated and encrypted communication paths.
- Application communication must be observable and auditable.
- Direct database-to-database integration is prohibited unless explicitly approved as a transition exception.
