# ItemTaxCode

Tax rate code

## Example Usage

```typescript
import { ItemTaxCode } from "crm/models/operations";

let value: ItemTaxCode = "VAT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"VAT" | "TAX_EXEMPT" | "SALES_TAX" | "OTHER" | Unrecognized<string>
```