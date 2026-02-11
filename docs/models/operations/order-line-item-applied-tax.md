# OrderLineItemAppliedTax

## Example Usage

```typescript
import { OrderLineItemAppliedTax } from "crm/models/operations";

let value: OrderLineItemAppliedTax = {
  taxRate: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    taxCode: "VAT",
    percentage: 1,
  },
  taxAmount: 0.99,
  taxExemptReason: "CONTACT",
};
```

## Fields

| Field                                                                                                   | Type                                                                                                    | Required                                                                                                | Description                                                                                             | Example                                                                                                 |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| `taxRate`                                                                                               | [operations.OrderLineItemTaxRate](../../models/operations/order-line-item-tax-rate.md)                  | :heavy_minus_sign:                                                                                      | N/A                                                                                                     |                                                                                                         |
| `taxAmount`                                                                                             | *number*                                                                                                | :heavy_minus_sign:                                                                                      | N/A                                                                                                     | 0.99                                                                                                    |
| `taxExemptReason`                                                                                       | [operations.OrderLineItemTaxExemptReason](../../models/operations/order-line-item-tax-exempt-reason.md) | :heavy_minus_sign:                                                                                      | N/A                                                                                                     | CONTACT                                                                                                 |