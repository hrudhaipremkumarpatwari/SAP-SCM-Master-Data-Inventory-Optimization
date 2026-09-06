# Data Mapping Strategy

## Purpose

The mapping strategy defines how source-system fields are translated into planning-relevant SAP SCM/APO master data. It also identifies validation rules so poor-quality data is not carried into the planning model.

## Example Source-to-Target Mapping

| Source field | SAP planning object / target | Validation |
|---|---|---|
| Material Code | Product | Unique, active, valid format |
| Material Description | Product description | Standard naming convention |
| Base UoM | Product UoM | Valid and convertible |
| Plant / DC Code | Location | Existing and correctly typed |
| Product + Location | Location-product | Valid combination |
| Supplier Code | Supplier location / sourcing relation | Approved supplier |
| Procurement Lead Time | Location-product / sourcing parameter | Positive, calendar-aware |
| Safety Stock | Location-product inventory parameter | Non-negative and segment-approved |
| Minimum Lot Size | Lot-size parameter | Consistent with pack/order constraints |
| Resource Capacity | Resource master | Valid unit and calendar |
| Source/Destination | Transportation lane | Both locations valid |
| Transit Time | Transportation lane | Positive and realistic |

## Cleansing Rules

1. Remove duplicate identifiers.
2. Standardize descriptions and code formats.
3. Convert units of measure into accepted standards.
4. Flag missing lead times, calendars, safety-stock values, and sourcing data.
5. Identify obsolete products and locations.
6. Reconcile supplier, plant, and distribution-center relationships.
7. Validate numeric ranges and date formats.

## Migration / Integration Checks

- Validate dependent master data before activating planning objects.
- Confirm product/location combinations exist before inventory parameters are loaded.
- Review CIF integration-model scope and filters before transfer.
- Reconcile record counts before and after transfer.
- Review error queues or transfer logs where applicable.
- Perform sample business validation after integration.

## Governance

Every critical field should have an owner, validation rule, change process, and review frequency. High-impact fields such as lead time, lot size, UoM, safety stock, sourcing, and transportation data require controlled changes because they directly influence planning output and inventory levels.
