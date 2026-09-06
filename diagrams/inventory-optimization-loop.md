# Inventory Optimization Loop

```mermaid
flowchart TD
    A[Demand & Inventory Data] --> B[Validate Master Data]
    B --> C[Segment Products]
    C --> D[Review Safety Stock / Lot Size / Lead Time]
    D --> E[Simulate Stock-out or Excess]
    E --> F[Apply Corrective Action]
    F --> G[Monitor KPIs]
    G --> H{Target Achieved?}
    H -- No --> D
    H -- Yes --> I[Standardize & Govern]
```

The loop illustrates how inventory parameters should be reviewed using demand, supply, and data-quality evidence, then monitored after changes rather than treated as fixed values.
