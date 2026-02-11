# OrderLineItemTaxRate

## Example Usage

```typescript
import { OrderLineItemTaxRate } from "crm/models/operations";

let value: OrderLineItemTaxRate = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  taxCode: "VAT",
  percentage: 1,
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            | Example                                                                                |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `id`                                                                                   | *string*                                                                               | :heavy_minus_sign:                                                                     | The entity identifier                                                                  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                   |
| `name`                                                                                 | *string*                                                                               | :heavy_minus_sign:                                                                     | N/A                                                                                    |                                                                                        |
| `taxCode`                                                                              | [operations.OrderLineItemTaxCode](../../models/operations/order-line-item-tax-code.md) | :heavy_minus_sign:                                                                     | N/A                                                                                    | VAT                                                                                    |
| `percentage`                                                                           | *number*                                                                               | :heavy_minus_sign:                                                                     | N/A                                                                                    | 1                                                                                      |