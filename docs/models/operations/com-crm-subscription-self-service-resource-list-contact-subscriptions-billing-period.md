# ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsBillingPeriod

The subscription's billing cycle duration

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsBillingPeriod } from "crm/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsBillingPeriod = {
    duration: 1,
    uot: "MONTH",
  };
```

## Fields

| Field                                                                                                                                                                               | Type                                                                                                                                                                                | Required                                                                                                                                                                            | Description                                                                                                                                                                         | Example                                                                                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `duration`                                                                                                                                                                          | *number*                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                  | The billing cycle's duration                                                                                                                                                        | 1                                                                                                                                                                                   |
| `uot`                                                                                                                                                                               | [operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsUot](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscriptions-uot.md) | :heavy_minus_sign:                                                                                                                                                                  | The billing cycle's unit of time                                                                                                                                                    | MONTH                                                                                                                                                                               |