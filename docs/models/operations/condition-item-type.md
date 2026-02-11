# ConditionItemType

The type of the product condition

## Example Usage

```typescript
import { ConditionItemType } from "crmcom/models/operations";

let value: ConditionItemType = "SKU";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SKU" | "TYPE" | "FAMILY" | "BRAND" | Unrecognized<string>
```