# Implementation Governance

## 1. Architecture Review

## Purpose

Ensure implementation remains aligned with approved architecture.

## Review Flow

```text
Change / Project Proposal
        ↓
Architecture Assessment
        ↓
Security / Data / Operations Review
        ↓
Architecture Decision
        ↓
Implementation
        ↓
Compliance Verification
```

## Review Checklist

- business requirement traceability
- architecture alignment
- security
- data ownership
- API/integration
- availability/resilience
- observability
- deployment
- cost
- operational support
- technical debt
- exception requirements

Review thresholds and approval authority are **To Validate**.

## 2. Exceptions

## Purpose

Document deviations from approved principles, standards or architecture decisions.

## Exception Record

Every exception should capture:

- request
- affected principle/standard
- reason
- business impact
- security impact
- operational impact
- cost impact
- risk
- compensating controls
- owner
- expiry/review date
- approval

## Lifecycle

```text
Exception Request
      ↓
Impact Assessment
      ↓
Architecture Review
      ↓
Approved / Rejected
      ↓
Compensating Controls
      ↓
Periodic Review
```

Exceptions should be time-bound where practical.
