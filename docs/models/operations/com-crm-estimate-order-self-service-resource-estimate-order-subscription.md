# ComCrmEstimateOrderSelfServiceResourceEstimateOrderSubscription

## Example Usage

```typescript
import { ComCrmEstimateOrderSelfServiceResourceEstimateOrderSubscription } from "crmcom/models/operations";

let value: ComCrmEstimateOrderSelfServiceResourceEstimateOrderSubscription = {
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

| Field                                                                                                                                                                                        | Type                                                                                                                                                                                         | Required                                                                                                                                                                                     | Description                                                                                                                                                                                  | Example                                                                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `state`                                                                                                                                                                                      | [operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderSubscriptionState](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-subscription-state.md) | :heavy_minus_sign:                                                                                                                                                                           | N/A                                                                                                                                                                                          | ACTIVE                                                                                                                                                                                       |
| `terms`                                                                                                                                                                                      | [operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderTerms](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-terms.md)                          | :heavy_minus_sign:                                                                                                                                                                           | N/A                                                                                                                                                                                          |                                                                                                                                                                                              |