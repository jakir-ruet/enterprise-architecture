# Architecture Change

## 1. Change Management

## Purpose

Phase H determines whether the architecture remains fit for purpose as business, technology, security and regulatory conditions change.

## Change Triggers

- new business capability
- major regulatory change
- new technology
- security requirement
- performance issue
- availability issue
- major cost change
- new external integration
- organizational change

## Change Lifecycle

```text
Change Trigger
      ↓
Architecture Impact Assessment
      ↓
Decision
      ↓
Approved Architecture Change
      ↓
New / Updated ADM Cycle
```

Architecture change should remain traceable to requirements and ADRs.

## 2. Change Request

## Template

### Request

- Change ID:
- Requester:
- Date:
- Description:

### Reason

- Business driver:
- Technology driver:
- Security driver:
- Regulatory driver:
- Operational driver:

### Affected Architecture

- Business:
- Data:
- Application:
- Technology:
- Security:
- Integration:

### Decision

- Proposed action:
- Decision:
- Decision owner:
- ADR reference:

### Implementation

- Migration impact:
- Dependencies:
- Risks:
- Rollback/recovery:
- Target date:

All fields should be completed according to the organization's governance process.

## 3. Impact Assessment

## Assessment Dimensions

| Dimension | Questions |
|---|---|
| Business | Which capabilities/processes change? |
| Data | Which data domains and flows change? |
| Application | Which applications/components change? |
| Technology | Which infrastructure/runtime components change? |
| Security | Which threats/controls change? |
| Integration | Which interfaces/contracts change? |
| Operations | Which monitoring/support processes change? |
| Cost | What is the implementation and operating cost impact? |
| Migration | What roadmap/wave changes are required? |
| Risk | What new or changed risks are introduced? |

## Outcome

The assessment should conclude with:

- no architecture change required
- update existing architecture
- create new architecture decision
- initiate a new ADM cycle
