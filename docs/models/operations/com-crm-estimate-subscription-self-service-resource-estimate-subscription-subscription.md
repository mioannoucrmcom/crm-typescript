# ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionSubscription

## Example Usage

```typescript
import { ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionSubscription } from "crm/models/operations";

let value:
  ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionSubscription =
    {
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

| Field                                                                                                                                                                                                                    | Type                                                                                                                                                                                                                     | Required                                                                                                                                                                                                                 | Description                                                                                                                                                                                                              | Example                                                                                                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `state`                                                                                                                                                                                                                  | [operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionSubscriptionState](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-subscription-subscription-state.md) | :heavy_minus_sign:                                                                                                                                                                                                       | N/A                                                                                                                                                                                                                      | ACTIVE                                                                                                                                                                                                                   |
| `terms`                                                                                                                                                                                                                  | [operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionTerms](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-subscription-terms.md)                          | :heavy_minus_sign:                                                                                                                                                                                                       | N/A                                                                                                                                                                                                                      |                                                                                                                                                                                                                          |