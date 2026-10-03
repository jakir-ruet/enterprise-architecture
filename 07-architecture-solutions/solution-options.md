# Solution Options

## Purpose

Evaluate alternative approaches before committing to a target solution.

## Example Options

### Option A — Improve Existing Application

```text
Existing ads-promo-web
        +
Existing ads-promo-api
        +
Improved security/observability/deployment
```

### Option B — Modularize the Backend

```text
ads-promo-api
   ├── Customer
   ├── Advertisement
   ├── Campaign
   ├── Promotion
   └── Messaging
```

### Option C — Selective Service Extraction

Extract only domains with a demonstrated need for independent scaling, deployment, ownership or resilience.

## Evaluation Criteria

- business value
- complexity
- delivery risk
- security
- scalability
- reliability
- operational effort
- migration effort
- total cost of ownership
- team capability

No option is approved by this document alone; approval belongs in the relevant architecture decision process.
