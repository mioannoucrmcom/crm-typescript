# InvoiceEstimateTaxesBreakdownTaxRate

The applied tax rate

## Example Usage

```typescript
import { InvoiceEstimateTaxesBreakdownTaxRate } from "crm/models/operations";

let value: InvoiceEstimateTaxesBreakdownTaxRate = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "VAT",
  taxCode: "VAT",
};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             | Example                                                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                    | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | The entity identifier                                                                                                   | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                    |
| `name`                                                                                                                  | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | Tax rate name                                                                                                           | VAT                                                                                                                     |
| `taxCode`                                                                                                               | [operations.InvoiceEstimateTaxesBreakdownTaxCode](../../models/operations/invoice-estimate-taxes-breakdown-tax-code.md) | :heavy_minus_sign:                                                                                                      | Tax rate code                                                                                                           | VAT                                                                                                                     |
| `percentage`                                                                                                            | *number*                                                                                                                | :heavy_minus_sign:                                                                                                      | The applied tax rate’s percentage that was valid on the date on which the rate was applied                              |                                                                                                                         |