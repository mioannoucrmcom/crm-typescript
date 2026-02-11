# InvoiceEstimateTaxesBreakdown

## Example Usage

```typescript
import { InvoiceEstimateTaxesBreakdown } from "crm/models/operations";

let value: InvoiceEstimateTaxesBreakdown = {
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
| `taxRate`                                                                                                                                                      | [operations.InvoiceEstimateTaxesBreakdownTaxRate](../../models/operations/invoice-estimate-taxes-breakdown-tax-rate.md)                                        | :heavy_minus_sign:                                                                                                                                             | The applied tax rate                                                                                                                                           |                                                                                                                                                                |
| `taxAmount`                                                                                                                                                    | *number*                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                             | The applied tax amount                                                                                                                                         | 1.5                                                                                                                                                            |
| `taxExemptReason`                                                                                                                                              | [operations.InvoiceEstimateTaxesBreakdownTaxExemptReason](../../models/operations/invoice-estimate-taxes-breakdown-tax-exempt-reason.md)                       | :heavy_minus_sign:                                                                                                                                             | Applicable only when a Tax Exempt rate was applied. Shows whether the tax exempt rate was applied because the Contact or the Product was marked as tax exempt. | PRODUCT                                                                                                                                                        |