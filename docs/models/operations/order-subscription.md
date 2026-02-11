# OrderSubscription

## Example Usage

```typescript
import { OrderSubscription } from "crmcom/models/operations";

let value: OrderSubscription = {
  state: "ACTIVE",
  terms: {
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
  },
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              | Example                                                                                  |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `state`                                                                                  | [operations.OrderSubscriptionState](../../models/operations/order-subscription-state.md) | :heavy_minus_sign:                                                                       | N/A                                                                                      | ACTIVE                                                                                   |
| `terms`                                                                                  | [operations.OrderTerms](../../models/operations/order-terms.md)                          | :heavy_minus_sign:                                                                       | N/A                                                                                      |                                                                                          |