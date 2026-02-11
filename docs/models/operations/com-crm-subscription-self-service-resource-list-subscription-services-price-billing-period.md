# ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesPriceBillingPeriod

How often the service is billed

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesPriceBillingPeriod } from "crm/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesPriceBillingPeriod =
    {
      duration: 1,
      uot: "MONTH",
    };
```

## Fields

| Field                                                                                                                                                                                          | Type                                                                                                                                                                                           | Required                                                                                                                                                                                       | Description                                                                                                                                                                                    | Example                                                                                                                                                                                        |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `duration`                                                                                                                                                                                     | *number*                                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                             | The billing cycle's duration                                                                                                                                                                   | 1                                                                                                                                                                                              |
| `uot`                                                                                                                                                                                          | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesPriceUot](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-price-uot.md) | :heavy_minus_sign:                                                                                                                                                                             | The billing cycle's unit of time                                                                                                                                                               | MONTH                                                                                                                                                                                          |