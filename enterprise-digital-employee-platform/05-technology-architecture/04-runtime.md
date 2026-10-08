# Runtime Architecture

## Runtime Layers

| Layer         | Responsibility            |
| ------------- | ------------------------- |
| Edge          | TLS termination / ingress |
| API           | API routing and policy    |
| Application   | Business services         |
| Messaging     | Asynchronous events       |
| Data          | Operational persistence   |
| Analytics     | Reporting workloads       |
| Observability | Logs, metrics, traces     |
| Security      | IAM, secrets, policy      |

## Deployment

```text
Source
 ↓
Git
 ↓
CI
 ↓
Build / Test / Scan
 ↓
Container Image
 ↓
Registry
 ↓
CD
 ↓
Kubernetes
 ↓
Monitoring
```
