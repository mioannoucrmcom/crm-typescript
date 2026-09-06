# ItemTaxExemptReason

Applicable only when a Tax Exempt rate was applied. Shows whether the tax exempt rate was applied because the Contact or the Product was marked as tax exempt.

## Example Usage

```typescript
import { ItemTaxExemptReason } from "crm/models/operations";

let value: ItemTaxExemptReason = "PRODUCT";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"CONTACT" | "PRODUCT" | Unrecognized<string>
```