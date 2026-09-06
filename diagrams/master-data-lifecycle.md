# Master Data Lifecycle

```mermaid
flowchart LR
    A[Source Data] --> B[Profile & Assess]
    B --> C[Clean & Standardize]
    C --> D[Map Source to Target]
    D --> E[Validate SAP Master Data]
    E --> F[Integrate / Migrate]
    F --> G[Planning & Inventory Use]
    G --> H[Monitor KPIs]
    H --> I[Govern & Correct]
    I --> B
```

This diagram represents the continuous master-data management cycle used in the Week 2 project. Data quality is treated as an ongoing governance process rather than a one-time migration activity.
