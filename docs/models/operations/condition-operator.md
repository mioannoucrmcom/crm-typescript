# ConditionOperator

## Example Usage

```typescript
import { ConditionOperator } from "crm/models/operations";

let value: ConditionOperator = "OR";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"AND" | "OR" | Unrecognized<string>
```