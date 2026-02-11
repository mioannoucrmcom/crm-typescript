# OfferingType

Defines whether the offering is an actual discount amount or a discount percentage

## Example Usage

```typescript
import { OfferingType } from "crm/models/operations";

let value: OfferingType = "PERCENT";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"AMOUNT" | "PERCENT" | Unrecognized<string>
```