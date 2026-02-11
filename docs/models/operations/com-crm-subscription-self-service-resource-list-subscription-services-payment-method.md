# ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesPaymentMethod

Payment method included in Get methods of Payments,Refunds and Payouts

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesPaymentMethod } from "crmcom/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesPaymentMethod = {
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
| `type`                                                                                                                                                                                        | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesType](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-type.md)         | :heavy_minus_sign:                                                                                                                                                                            | Available payment method types                                                                                                                                                                | CARD                                                                                                                                                                                          |
| `identity`                                                                                                                                                                                    | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesIdentity](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-identity.md) | :heavy_minus_sign:                                                                                                                                                                            | Payment method details                                                                                                                                                                        |                                                                                                                                                                                               |