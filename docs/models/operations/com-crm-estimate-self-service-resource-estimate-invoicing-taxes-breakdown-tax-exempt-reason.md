# ComCrmEstimateSelfServiceResourceEstimateInvoicingTaxesBreakdownTaxExemptReason

Applicable only when a Tax Exempt rate was applied. Shows whether the tax exempt rate was applied because the Contact or the Product was marked as tax exempt.

## Example Usage

```typescript
import { ComCrmEstimateSelfServiceResourceEstimateInvoicingTaxesBreakdownTaxExemptReason } from "crm/models/operations";

let value:
  ComCrmEstimateSelfServiceResourceEstimateInvoicingTaxesBreakdownTaxExemptReason =
    "PRODUCT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"CONTACT" | "PRODUCT" | Unrecognized<string>
```