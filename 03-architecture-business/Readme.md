# Business Architecture

## 1. Capabilities

## Capability Map

```text
Ads Promotional Management
├── Customer Management
├── Advertisement Management
├── Media Management
├── Campaign Management
├── Promotion Management
├── Reporting
├── Audit
├── User & Access Management
└── Customer Messaging
```

## Capability Maturity

Capability maturity should be assessed against business objectives and actual implementation.

| Capability                 | Current implementation    | Target assessment |
| -------------------------- | ------------------------- | ----------------- |
| Customer Management        | Confirmed as system scope | To Validate       |
| Advertisement Management   | Confirmed as system scope | To Validate       |
| Campaign Management        | Confirmed as system scope | To Validate       |
| Promotion Management       | Confirmed as system scope | To Validate       |
| Reporting                  | Confirmed as system scope | To Validate       |
| Audit                      | Confirmed as system scope | To Validate       |
| User/Permission Management | Confirmed as system scope | To Validate       |
| WhatsApp-related messaging | Confirmed as system scope | To Validate       |

## 2. Business Services

## Candidate Business Services

| Business service         | Description                                 | Status      |
| ------------------------ | ------------------------------------------- | ----------- |
| Customer Management      | Maintain customer-related information       | To Validate |
| Advertisement Management | Manage advertisements                       | To Validate |
| Campaign Management      | Manage campaigns                            | To Validate |
| Promotion Management     | Manage promotional activities               | To Validate |
| Media Management         | Manage advertisement media                  | To Validate |
| Reporting                | Provide operational/business reporting      | To Validate |
| Audit                    | Provide traceability of relevant activities | To Validate |
| Access Management        | Manage users, roles and permissions         | To Validate |
| Customer Messaging       | Support customer messaging capabilities     | To Validate |

These are architecture-level service boundaries, not necessarily independent microservices.

## 3. Processes

## Working Process Model

```text
Customer / Business Input
        ↓
Advertisement / Campaign Setup
        ↓
Media / Promotion Configuration
        ↓
Approval / Validation
        ↓
Publication / Execution
        ↓
Customer Messaging / Engagement
        ↓
Monitoring / Reporting
        ↓
Audit
```

This is a working architecture-level process view. Exact workflow states, approval rules and ownership must be validated against the application implementation and business process documentation.
