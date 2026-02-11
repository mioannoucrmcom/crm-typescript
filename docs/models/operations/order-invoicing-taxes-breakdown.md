# OrderInvoicingTaxesBreakdown

## Example Usage

```typescript
import { OrderInvoicingTaxesBreakdown } from "crmcom/models/operations";

let value: OrderInvoicingTaxesBreakdown = {
  taxRate: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    taxCode: "VAT",
    percentage: 1,
  },
  taxAmount: 0.99,
};
```

## Fields

| Field                                                                                                                 | Type                                                                                                                  | Required                                                                                                              | Description                                                                                                           | Example                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `taxRate`                                                                                                             | [operations.OrderInvoicingTaxesBreakdownTaxRate](../../models/operations/order-invoicing-taxes-breakdown-tax-rate.md) | :heavy_minus_sign:                                                                                                    | N/A                                                                                                                   |                                                                                                                       |
| `taxAmount`                                                                                                           | *number*                                                                                                              | :heavy_minus_sign:                                                                                                    | N/A                                                                                                                   | 0.99                                                                                                                  |