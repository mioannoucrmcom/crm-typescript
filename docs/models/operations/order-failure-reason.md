# OrderFailureReason

Shows the reason why the order cannot be placed

## Example Usage

```typescript
import { OrderFailureReason } from "crmcom/models/operations";

let value: OrderFailureReason = "MINIMUM_COST";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"MINIMUM_COST" | "TAX_CALCULATION" | Unrecognized<string>
```