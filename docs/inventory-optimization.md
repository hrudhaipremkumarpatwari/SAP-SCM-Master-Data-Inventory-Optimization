# Inventory Optimization Approach

## Objective

The inventory approach balances customer service with working-capital and storage considerations. The recommendations are illustrative and should be validated against real demand variability, replenishment performance, and business policy before implementation.

## Techniques

### Safety Stock / Safety Days
Safety stock protects against demand or supply variability. The buffer should be reviewed using demand volatility, replenishment lead time, supplier reliability, and required service level rather than applying one value to every product.

### Reorder Point
A simple reorder-point concept can be expressed as:

`Reorder Point = Expected demand during lead time + Safety stock`

### Economic Order Quantity (EOQ)
EOQ can help compare ordering cost and holding cost when assumptions are reasonably stable:

`EOQ = sqrt((2 × Annual Demand × Ordering Cost) / Annual Holding Cost per Unit)`

### ABC-XYZ Segmentation
- **ABC:** classifies products by business/inventory value.
- **XYZ:** classifies products by demand variability or predictability.

Combining the two allows differentiated planning. For example, AX items may receive tight service and replenishment control, while CZ items may require cautious stocking because demand is intermittent.

### Lot-Size Review
Minimum, maximum, fixed, and rounding quantities should reflect real pack sizes and supplier constraints. Oversized lots can create excess stock, while very small lots can increase ordering and transport activity.

### Redeployment and Dual Sourcing
When one location has excess stock and another faces shortage, redeployment may reduce urgent procurement. Dual sourcing can reduce dependency on one supplier where the cost and qualification requirements justify it.

## Simulation 1: Stock-out Risk

**Situation:** A transport delay extends replenishment lead time while demand continues at the expected rate.

**Possible root causes:** insufficient buffer, outdated lead time, single-source dependency, or delayed planning response.

**Proposed actions:** review safety stock, correct lead time, evaluate alternate sourcing or transport, prioritize available inventory, and increase monitoring frequency.

## Simulation 2: Excess Inventory

**Situation:** Demand falls below plan while replenishment continues in large lots.

**Possible root causes:** oversized lot size, stale forecast, high safety stock, or slow parameter review.

**Proposed actions:** reduce future lot sizes, review forecast and safety stock, redeploy usable stock, pause or reschedule receipts where possible, and monitor days of supply.

## Monitoring KPIs

| KPI | What it indicates |
|---|---|
| Fill rate / service level | Ability to satisfy demand |
| Stock-out frequency | Shortage exposure |
| Inventory days of supply | Coverage relative to demand |
| Excess inventory | Over-stocking risk |
| Lead-time adherence | Reliability of replenishment assumptions |
| Safety-stock exceptions | Buffer adequacy |
| Forecast/consumption variance | Demand-plan alignment |
| Master-data error rate | Planning-input quality |

## Review Cycle

High-value or volatile products should be reviewed more frequently than stable low-impact items. Parameter changes should be documented, approved by the responsible owner, tested in a planning/simulation context where possible, and monitored after implementation.
