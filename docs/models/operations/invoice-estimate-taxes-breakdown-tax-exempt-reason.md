# InvoiceEstimateTaxesBreakdownTaxExemptReason

Applicable only when a Tax Exempt rate was applied. Shows whether the tax exempt rate was applied because the Contact or the Product was marked as tax exempt.

## Example Usage

```typescript
import { InvoiceEstimateTaxesBreakdownTaxExemptReason } from "crm/models/operations";

let value: InvoiceEstimateTaxesBreakdownTaxExemptReason = "PRODUCT";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"CONTACT" | "PRODUCT" | Unrecognized<string>
```