# Requirements Impact Assessment

## Purpose

Assess changes to architecture requirements and determine their impact on the current architecture, in-progress ADM work, implementation scope, and future ADM cycles.

## Current Assessment

| Requirement | Change / Trigger | Impacted Area | Impact | Response | Status |
| ----------- | ---------------- | ------------- | ------ | -------- | ------ |
| AR-006 | API governance becomes mandatory for all new integrations | Application / Technology | High | Enforce API standards, lifecycle and review gates | Open |
| AR-008 | Enterprise SSO is required for all employee-facing services | Application / Security | High | Central IAM and migration of legacy authentication | Open |
| AR-010 | Critical-service availability target set at 99.9% | Technology / Operations | High | Multi-zone design, monitoring, backup and DR testing | Open |
| AR-012 | Formal DR capability required for critical services | Technology / Migration | High | Define RPO/RTO, backup and recovery tests | Open |
| AR-013 | Migration must avoid business disruption | Migration | High | Use transition architectures and incremental cutover | Open |

## Impact Assessment Method

```text
Changed Requirement
        ↓
Identify affected stakeholders
        ↓
Assess impact on current / target architecture
        ↓
Assess impact on ADM phase and roadmap
        ↓
Update requirements and affected artifacts
        ↓
Record decision / action
        ↓
Update repository and traceability
```

## Impacted Artifacts

- Architecture Vision
- Business / Data / Application / Technology Baseline and Target views
- Gap Register
- Work Packages
- Transition Architectures
- Architecture Roadmap
- Implementation and Migration Plan
- Architecture Contract / Compliance Assessment

## Requirements Impact Statement

The current assessment confirms that security, availability, integration governance and incremental migration requirements materially influence the target architecture and roadmap. These requirements must remain traceable through implementation governance and future architecture change cycles.

## Governance Rule

Requirements Management remains continuous. A material requirement change must trigger an impact assessment before affected architecture decisions, work packages or implementation plans are approved.
