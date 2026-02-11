# ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsPaymentMethod

The subscription's payment method

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsPaymentMethod } from "crmcom/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsPaymentMethod = {
    type: "CARD",
    identity: {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      identifier: "Visa *****1234 03/25",
    },
  };
```

## Fields

| Field                                                                                                                                                                                         | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   | Example                                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                                                                                                                                                                                        | [operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsType](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscriptions-type.md)         | :heavy_minus_sign:                                                                                                                                                                            | Available payment method types                                                                                                                                                                | CARD                                                                                                                                                                                          |
| `identity`                                                                                                                                                                                    | [operations.ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsIdentity](../../models/operations/com-crm-subscription-self-service-resource-list-contact-subscriptions-identity.md) | :heavy_minus_sign:                                                                                                                                                                            | Payment method details                                                                                                                                                                        |                                                                                                                                                                                               |