# VariableDiscountType

Defines whether the offering is an actual discount amount or a discount percentage

## Example Usage

```typescript
import { VariableDiscountType } from "crm/models/operations";

let value: VariableDiscountType = "PERCENT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"AMOUNT" | "PERCENT" | Unrecognized<string>
```