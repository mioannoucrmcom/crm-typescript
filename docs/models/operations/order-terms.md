# OrderTerms

## Example Usage

```typescript
import { OrderTerms } from "crmcom/models/operations";

let value: OrderTerms = {
  billingPeriod: {
    duration: 1,
    uot: "MONTH",
  },
  billingDay: {
    dayOfWeek: "MONDAY",
    dayOfMonth: 5,
    monthOfYear: "JANUARY",
  },
  billingModel: "PRE_BILL",
};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      | Example                                                                          |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `billingPeriod`                                                                  | [operations.OrderBillingPeriod](../../models/operations/order-billing-period.md) | :heavy_minus_sign:                                                               | N/A                                                                              |                                                                                  |
| `billingDay`                                                                     | [operations.OrderBillingDay](../../models/operations/order-billing-day.md)       | :heavy_minus_sign:                                                               | N/A                                                                              |                                                                                  |
| `billingModel`                                                                   | [operations.OrderBillingModel](../../models/operations/order-billing-model.md)   | :heavy_minus_sign:                                                               | N/A                                                                              | PRE_BILL                                                                         |