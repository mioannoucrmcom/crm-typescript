# ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSubscriptionBillingPeriod

How often services are billed

## Example Usage

```typescript
import {
  ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSubscriptionBillingPeriod,
} from "crmcom/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSubscriptionBillingPeriod =
    {
      duration: 1,
      uot: "MONTH",
    };
```

## Fields

| Field                                                                                                                                                                                                        | Type                                                                                                                                                                                                         | Required                                                                                                                                                                                                     | Description                                                                                                                                                                                                  | Example                                                                                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `duration`                                                                                                                                                                                                   | *number*                                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                           | The billing cycle's duration                                                                                                                                                                                 | 1                                                                                                                                                                                                            |
| `uot`                                                                                                                                                                                                        | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSubscriptionUot](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-subscription-uot.md) | :heavy_minus_sign:                                                                                                                                                                                           | The billing cycle's unit of time                                                                                                                                                                             | MONTH                                                                                                                                                                                                        |