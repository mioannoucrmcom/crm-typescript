# OrderInvoiceEstimateTaxesBreakdown

## Example Usage

```typescript
import { OrderInvoiceEstimateTaxesBreakdown } from "crmcom/models/operations";

let value: OrderInvoiceEstimateTaxesBreakdown = {
  taxRate: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "VAT",
    taxCode: "VAT",
  },
  taxAmount: 1.5,
  taxExemptReason: "PRODUCT",
};
```

## Fields

| Field                                                                                                                                                          | Type                                                                                                                                                           | Required                                                                                                                                                       | Description                                                                                                                                                    | Example                                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `taxRate`                                                                                                                                                      | [operations.OrderInvoiceEstimateTaxesBreakdownTaxRate](../../models/operations/order-invoice-estimate-taxes-breakdown-tax-rate.md)                             | :heavy_minus_sign:                                                                                                                                             | The applied tax rate                                                                                                                                           |                                                                                                                                                                |
| `taxAmount`                                                                                                                                                    | *number*                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                             | The applied tax amount                                                                                                                                         | 1.5                                                                                                                                                            |
| `taxExemptReason`                                                                                                                                              | [operations.OrderTaxesBreakdownTaxExemptReason](../../models/operations/order-taxes-breakdown-tax-exempt-reason.md)                                            | :heavy_minus_sign:                                                                                                                                             | Applicable only when a Tax Exempt rate was applied. Shows whether the tax exempt rate was applied because the Contact or the Product was marked as tax exempt. | PRODUCT                                                                                                                                                        |