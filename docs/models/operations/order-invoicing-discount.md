# OrderInvoicingDiscount

## Example Usage

```typescript
import { OrderInvoicingDiscount } from "crmcom/models/operations";

let value: OrderInvoicingDiscount = {
  amount: 2,
  type: "AD_HOC",
  promotion: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Universal Name",
  },
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                | Example                                                                                    |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `amount`                                                                                   | *number*                                                                                   | :heavy_minus_sign:                                                                         | The deducted amount                                                                        | 2                                                                                          |
| `type`                                                                                     | [operations.OrderInvoicingType](../../models/operations/order-invoicing-type.md)           | :heavy_minus_sign:                                                                         | Type of discount applied                                                                   | AD_HOC                                                                                     |
| `promotion`                                                                                | [operations.OrderInvoicingPromotion](../../models/operations/order-invoicing-promotion.md) | :heavy_minus_sign:                                                                         | The applied Promotion. Applicable when discount type is Promotion                          |                                                                                            |