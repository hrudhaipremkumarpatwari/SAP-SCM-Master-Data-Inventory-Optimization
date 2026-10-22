# Risk and Validation Plan — Week 2

## Key risks
- Missing or incorrect master-data attributes can distort planning results.
- Unit conversions, lead times, lot sizes, or planning calendars can be inconsistent.
- Excess inventory can be reduced too aggressively and increase stock-out risk.
- Safety-stock or reorder parameters can be applied without segment-level review.
- Source-to-target mapping errors can create duplicate or missing planning objects.
- Simulated improvements can be mistaken for measured business benefits.

## Proposed validation tests

| ID | Check | Expected evidence |
|---|---|---|
| W2-V01 | Master-data completeness | Required material/location/planning fields are populated |
| W2-V02 | Mapping reconciliation | Source and target records match on controlled keys |
| W2-V03 | Unit conversion | Base and alternate units reproduce approved quantities |
| W2-V04 | Lead-time/calendar check | Planning dates reflect approved lead times and working calendars |
| W2-V05 | Safety-stock calculation | Parameter inputs and formula are documented and reproducible |
| W2-V06 | Stock-out scenario | Shortage risk is visible when inventory falls below the modeled requirement |
| W2-V07 | Excess-stock scenario | Excess inventory is identified without hiding service-impacting constraints |
| W2-V08 | Change-control approval | Parameter changes have an owner, reason, evidence and approval |
| W2-V09 | Post-change monitoring | Inventory and service KPIs are compared before and after a controlled change |

## Governance
Use a governed master-data owner, controlled mappings, documented approvals, and periodic exception review. These checks are proposed validation steps for the internship assessment and are not claims of production execution.
