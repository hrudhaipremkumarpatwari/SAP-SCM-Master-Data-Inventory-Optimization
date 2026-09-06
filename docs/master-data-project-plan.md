# Master Data Management Project Plan

## Scope

The project focuses on planning-relevant master data used by SAP SCM/APO for inventory and supply planning. The scope includes product, location, location-product, resource, sourcing, transportation, calendar, lead-time, unit-of-measure, safety-stock, and lot-size information.

## Project Phases

| Phase | Main activities | Output |
|---|---|---|
| 1. Assess | Identify sources and business owners | Data inventory |
| 2. Profile | Check completeness, duplicates, formats, ranges | Data-quality report |
| 3. Clean | Correct duplicates, invalid values, naming and UoM issues | Cleansed dataset |
| 4. Map | Define source-to-target field relationships | Mapping specification |
| 5. Validate | Check SAP object dependencies and business rules | Validation checklist |
| 6. Integrate | Review CIF integration-model requirements | Integration blueprint |
| 7. Optimize | Review inventory parameters and segmentation | Parameter recommendations |
| 8. Monitor | Track data and inventory KPIs | Monitoring plan |
| 9. Govern | Assign ownership and change controls | Governance model |

## Data Quality Rules

- Product and location identifiers must be unique.
- Units of measure must be standardized and convertible.
- Lead times must be positive, realistic, and consistent with business calendars.
- Transportation lanes must connect valid source and destination locations.
- Product/location combinations must exist before planning parameters are maintained.
- Safety stock and lot-size parameters should be reviewed by segment and service requirement.
- Duplicate or obsolete master records should be blocked or retired according to governance rules.

## Roles

- **Business owner:** validates business meaning and acceptable values.
- **Master-data steward:** cleans, standardizes, and controls changes.
- **SAP functional analyst:** maps fields to SAP/APO objects and validates dependencies.
- **Planner/procurement user:** confirms planning impact and operational usability.
- **IT/integration team:** supports interface and CIF integration controls.

## Estimated Effort

The task is designed as a 30-35 hour internship exercise. A reasonable allocation is 5 hours for research and profiling, 6 hours for cleansing and mapping, 7 hours for SAP configuration analysis, 6 hours for inventory optimization and simulations, 4 hours for KPI/risk analysis, and 5 hours for report preparation and review.
