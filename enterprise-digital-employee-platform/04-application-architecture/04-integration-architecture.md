# Integration Architecture

## Target Pattern

```mermaid
flowchart LR
    PORTAL[Portal]
    API[API Gateway]
    SVC[Business Services]
    BUS[Message / Event Bus]
    LEGACY[Legacy HR / Payroll]
    DATA[Data Platform]

    PORTAL --> API
    API --> SVC
    SVC --> BUS
    BUS --> LEGACY
    LEGACY --> BUS
    BUS --> DATA
```

## Integration Patterns

| Pattern              | Use                                            |
| -------------------- | ---------------------------------------------- |
| Synchronous REST API | Immediate request/response                     |
| Asynchronous Event   | Decoupled business event                       |
| Batch                | Controlled bulk transfer                       |
| File exchange        | Temporary legacy integration where unavoidable |

## Rule

Prefer governed APIs/events over uncontrolled point-to-point integration.
