# Application Integration

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
