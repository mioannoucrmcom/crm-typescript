# OrderItemTaxRate

The applied tax rate

## Example Usage

```typescript
import { OrderItemTaxRate } from "crm/models/operations";

let value: OrderItemTaxRate = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "VAT",
  taxCode: "VAT",
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                | Example                                                                                    |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `id`                                                                                       | *string*                                                                                   | :heavy_minus_sign:                                                                         | The entity identifier                                                                      | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                       |
| `name`                                                                                     | *string*                                                                                   | :heavy_minus_sign:                                                                         | Tax rate name                                                                              | VAT                                                                                        |
| `taxCode`                                                                                  | [operations.OrderItemTaxCode](../../models/operations/order-item-tax-code.md)              | :heavy_minus_sign:                                                                         | Tax rate code                                                                              | VAT                                                                                        |
| `percentage`                                                                               | *number*                                                                                   | :heavy_minus_sign:                                                                         | The applied tax rate’s percentage that was valid on the date on which the rate was applied |                                                                                            |