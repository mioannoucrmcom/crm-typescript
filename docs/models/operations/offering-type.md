# OfferingType

Defines whether the offering is an actual discount amount or a discount percentage

## Example Usage

```typescript
import { OfferingType } from "crm/models/operations";

let value: OfferingType = "PERCENT";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"AMOUNT" | "PERCENT" | Unrecognized<string>
```