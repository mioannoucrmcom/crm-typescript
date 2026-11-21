# VariableDiscountType

Defines whether the offering is an actual discount amount or a discount percentage

## Example Usage

```typescript
import { VariableDiscountType } from "crm/models/operations";

let value: VariableDiscountType = "PERCENT";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"AMOUNT" | "PERCENT" | Unrecognized<string>
```