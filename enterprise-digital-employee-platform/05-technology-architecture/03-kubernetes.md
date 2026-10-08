# Kubernetes Architecture

## Target Runtime Scenario

Kubernetes is selected as a target application runtime **for this training scenario**, subject to architecture governance and technology trade-off review.

```text
Ingress
  ↓
API Gateway / Ingress Controller
  ↓
Kubernetes
├── portal
├── hr-service
├── leave-service
├── performance-service
├── recruitment-service
├── notification-service
└── integration-service
  ↓
Managed Data Services
```

## Kubernetes Requirements

- Namespace separation
- Resource requests/limits
- Horizontal scaling
- Pod disruption controls
- Health probes
- Secret management
- Network policies
- Ingress controls
- Central logs/metrics
- Rolling deployment
- Image scanning
- RBAC

## Operational Rule

Kubernetes is an enabling technology, not the architecture objective. Business requirements remain the driver.
