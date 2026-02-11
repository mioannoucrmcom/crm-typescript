# ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSubscription

The subscription of the service

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSubscription } from "crm/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSubscription = {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    code: "60012321123",
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
      paymentMethod: {
        type: "CARD",
        identity: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          identifier: "Visa *****1234 03/25",
        },
      },
      billingModel: "PRE_BILL",
    },
  };
```

## Fields

| Field                                                                                                                                                                                                            | Type                                                                                                                                                                                                             | Required                                                                                                                                                                                                         | Description                                                                                                                                                                                                      | Example                                                                                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                                             | *string*                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                               | The entity identifier                                                                                                                                                                                            | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                             |
| `code`                                                                                                                                                                                                           | *string*                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                               | Subscription code                                                                                                                                                                                                | 60012321123                                                                                                                                                                                                      |
| `terms`                                                                                                                                                                                                          | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSubscriptionTerms](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-subscription-terms.md) | :heavy_minus_sign:                                                                                                                                                                                               | N/A                                                                                                                                                                                                              |                                                                                                                                                                                                                  |
| `state`                                                                                                                                                                                                          | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSubscriptionState](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-subscription-state.md) | :heavy_minus_sign:                                                                                                                                                                                               | The subscription's state                                                                                                                                                                                         |                                                                                                                                                                                                                  |