# Data Model

## Conceptual Model

```mermaid
erDiagram
    ORGANIZATION ||--o{ EMPLOYEE : contains
    POSITION ||--o{ EMPLOYMENT : assigned
    EMPLOYEE ||--o{ EMPLOYMENT : has
    EMPLOYEE ||--o{ PAYROLL : receives
    EMPLOYEE ||--o{ LEAVE : requests
    EMPLOYEE ||--o{ ATTENDANCE : records
    EMPLOYEE ||--o{ PERFORMANCE : receives
    EMPLOYEE ||--o{ BENEFIT : receives
    EMPLOYEE ||--o{ CANDIDATE : "may originate"
```

## Logical Model Principles

- Surrogate enterprise identifiers where required.
- Clear ownership of master data.
- Referential integrity.
- Temporal handling for employment and organizational changes.
- Audit fields on critical records.
- Classification of sensitive attributes.
- Separate operational and analytical workloads.

## Data Lifecycle

```text
Create → Validate → Use → Share → Archive → Dispose
```
