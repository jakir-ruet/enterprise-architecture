# Application Architecture

## 1. Application Landscape

## Current Application Boundary

| Application        | Role                           | Status                                                       |
| ------------------ | ------------------------------ | ------------------------------------------------------------ |
| `ads-promo-web`    | Frontend / UI                  | Confirmed                                                    |
| `ads-promo-api`    | Backend / API                  | Confirmed                                                    |
| Database           | Persistence                    | Confirmed as a conceptual dependency; technology To Validate |
| ERP/CRM            | External integration           | To Validate                                                  |
| WhatsApp/Messaging | External messaging capability  | To Validate                                                  |
| Reporting/BI       | Reporting/analytics capability | To Validate                                                  |

## Important

Business capabilities should not automatically become separate applications or microservices. Application boundaries should be justified by business, operational and technical requirements.

## 2. Components

## Backend Logical Components

The following are architecture-level component candidates:

```text
ads-promo-api
├── Authentication / Authorization
├── Customer Management
├── Advertisement Management
├── Media Management
├── Campaign Management
├── Promotion Management
├── Reporting
├── Audit
└── Messaging / WhatsApp
```

These are logical boundaries and must not be interpreted as confirmed Java packages, modules or microservices until verified against the source repository.

## Frontend

```text
ads-promo-web
├── Authentication
├── Dashboard
├── Customer
├── Advertisement
├── Media
├── Campaign
├── Promotion
├── Reporting
├── Audit
├── User / Role / Permission
└── Messaging
```

Exact frontend modules are **To Validate**.

## 3. Integration

## Working Integration Model

```text
ads-promo-web
       │
       │ HTTPS/REST
       ▼
ads-promo-api
       │
       ├──── Database
       │
       ├──── ERP / CRM
       │
       ├──── WhatsApp / Messaging
       │
       └──── Reporting / BI
```

## Integration Principles

- Prefer documented contracts.
- Authenticate external calls.
- Apply authorization appropriate to the operation.
- Validate input and output.
- Use timeouts and controlled retry behavior where appropriate.
- Avoid tightly coupling business logic to external provider-specific behavior.
- Record integration failures and operational metrics.

Exact protocols, endpoints and providers are **To Validate**.
