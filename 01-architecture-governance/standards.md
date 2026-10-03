# Architecture Standards

This document defines the working standards baseline. Specific organizational standards must be confirmed against the enterprise technology and security standards.

## Application

- Clear separation between presentation, application/business logic and persistence.
- API contracts should be documented.
- Version APIs when backward-incompatible changes are required.
- Validate inputs at trust boundaries.
- Use centralized error handling and consistent response conventions.

## Security

- Use strong authentication and authorization controls.
- Protect secrets outside source code.
- Use TLS for sensitive network communication.
- Apply least privilege.
- Record security-relevant events where required.

## Data

- Define ownership for critical data.
- Protect sensitive data at rest and in transit.
- Apply data retention requirements.
- Avoid unnecessary duplication of authoritative data.

## Operations

- Centralize application logs where practical.
- Establish service health monitoring.
- Automate deployments where practical.
- Maintain rollback/recovery procedures.

## Architecture Documentation

- Use Markdown for textual architecture artifacts.
- Use ADRs for material architecture decisions.
- Mark uncertain information as `TBD` or `To Validate`.
