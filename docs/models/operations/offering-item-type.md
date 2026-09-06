# OfferingItemType

Determines on which product the discount will be applied.

## Example Usage

```typescript
import { OfferingItemType } from "crm/models/operations";

let value: OfferingItemType = "TYPE";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"SKU" | "TYPE" | "FAMILY" | "BRAND" | Unrecognized<string>
```