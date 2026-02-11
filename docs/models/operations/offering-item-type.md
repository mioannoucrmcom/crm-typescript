# OfferingItemType

Determines on which product the discount will be applied.

## Example Usage

```typescript
import { OfferingItemType } from "crm/models/operations";

let value: OfferingItemType = "TYPE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SKU" | "TYPE" | "FAMILY" | "BRAND" | Unrecognized<string>
```