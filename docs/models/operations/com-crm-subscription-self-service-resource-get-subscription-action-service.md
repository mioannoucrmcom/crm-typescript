# ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionService

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionService } from "crm/models/operations";

let value: ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionService = {
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
  price: {
    billingPeriod: {
      duration: 1,
      uot: "MONTH",
    },
  },
};
```

## Fields

| Field                                                                                                                                                                                                | Type                                                                                                                                                                                                 | Required                                                                                                                                                                                             | Description                                                                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `changeType`                                                                                                                                                                                         | [operations.ServiceChangeType](../../models/operations/service-change-type.md)                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                                   | N/A                                                                                                                                                                                                  |
| `product`                                                                                                                                                                                            | [operations.ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionServiceProduct](../../models/operations/com-crm-subscription-self-service-resource-get-subscription-action-service-product.md) | :heavy_minus_sign:                                                                                                                                                                                   | N/A                                                                                                                                                                                                  |
| `quantity`                                                                                                                                                                                           | *number*                                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                   | N/A                                                                                                                                                                                                  |
| `price`                                                                                                                                                                                              | [operations.ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionPrice](../../models/operations/com-crm-subscription-self-service-resource-get-subscription-action-price.md)                    | :heavy_minus_sign:                                                                                                                                                                                   | N/A                                                                                                                                                                                                  |