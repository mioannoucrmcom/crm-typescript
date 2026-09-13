# OrderFailureReason

Shows the reason why the order cannot be placed

## Example Usage

```typescript
import { OrderFailureReason } from "crm/models/operations";

let value: OrderFailureReason = "MINIMUM_COST";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"MINIMUM_COST" | "TAX_CALCULATION" | Unrecognized<string>
```