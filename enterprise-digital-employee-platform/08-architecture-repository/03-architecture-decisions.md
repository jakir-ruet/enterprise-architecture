# Architecture Decision Records

## ADR-001 — Unified Employee Portal

**Decision:** Create a single digital employee experience.

**Alternatives:** Separate portals / single portal.

**Reason:** Better user experience and reduced channel fragmentation.

## ADR-002 — API + Event Integration

**Decision:** Use governed APIs for synchronous needs and events for suitable asynchronous integration.

**Reason:** Reduce coupling and support reusable integration.

## ADR-003 — Kubernetes Runtime

**Decision:** Use Kubernetes as the target runtime scenario for this training architecture.

**Reason:** Supports containerized services, controlled deployment, scaling and platform standardization.

**Condition:** Final production selection remains subject to cost, skills, operational maturity, security, availability and workload trade-off analysis.

## ADR-004 — Central IAM

**Decision:** Centralize identity and access.

**Reason:** Consistent authentication, authorization and auditability.

## ADR-005 — Incremental Migration

**Decision:** Use Transition Architectures rather than a big-bang replacement.

**Reason:** Reduce business disruption and manage legacy dependencies.
