# Cloud Architecture

## Target Cloud Pattern

A cloud deployment is used as the target technology scenario for this training project.

```text
Cloud Landing Zone
├── Identity / IAM
├── Network
│   ├── Public / Edge
│   └── Private Application / Data
├── Compute
├── Data
├── Security
├── Observability
└── Backup / DR
```

## Cloud Principles

- Least privilege
- Private-by-default data services
- Multi-zone resilience for critical workloads
- Encryption in transit and at rest
- Centralized logging
- Infrastructure as Code
- Cost tagging
- Automated backup
- Tested recovery

> AWS services can be mapped to this architecture during the technology selection exercise. The architecture does not assume a particular vendor until requirements and trade-offs are reviewed.
