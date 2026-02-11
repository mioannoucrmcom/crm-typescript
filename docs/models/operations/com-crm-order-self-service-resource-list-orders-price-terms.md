# ComCrmOrderSelfServiceResourceListOrdersPriceTerms

The price terms of the ordered item. Applicable only when ordering termed and one-time services

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceListOrdersPriceTerms } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourceListOrdersPriceTerms = {
  billingPeriod: {
    duration: 1,
    uot: "MONTH",
  },
};
```

## Fields

| Field                                                                                                                                                         | Type                                                                                                                                                          | Required                                                                                                                                                      | Description                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `billingPeriod`                                                                                                                                               | [operations.ComCrmOrderSelfServiceResourceListOrdersBillingPeriod](../../models/operations/com-crm-order-self-service-resource-list-orders-billing-period.md) | :heavy_minus_sign:                                                                                                                                            | N/A                                                                                                                                                           |
| `autoRenew`                                                                                                                                                   | *boolean*                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                            | N/A                                                                                                                                                           |