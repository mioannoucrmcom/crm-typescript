# OrderOrderFailureReason

Shows the reason why the order cannot be placed

## Example Usage

```typescript
import { OrderOrderFailureReason } from "crm/models/operations";

let value: OrderOrderFailureReason = "MINIMUM_COST";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"MINIMUM_COST" | "TAX_CALCULATION" | Unrecognized<string>
```