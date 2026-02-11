# OrderBillingPeriod

## Example Usage

```typescript
import { OrderBillingPeriod } from "crmcom/models/operations";

let value: OrderBillingPeriod = {
  duration: 1,
  uot: "MONTH",
};
```

## Fields

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               | Example                                                                                   |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `duration`                                                                                | *number*                                                                                  | :heavy_minus_sign:                                                                        | The billing cycle's duration                                                              | 1                                                                                         |
| `uot`                                                                                     | [operations.OrderUotTaxCalculation](../../models/operations/order-uot-tax-calculation.md) | :heavy_minus_sign:                                                                        | The billing cycle's unit of time                                                          | MONTH                                                                                     |