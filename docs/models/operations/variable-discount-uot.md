# VariableDiscountUot

The period’s unit of time

## Example Usage

```typescript
import { VariableDiscountUot } from "crm/models/operations";

let value: VariableDiscountUot = "MONTH";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SECOND" | "MINUTE" | "HOUR" | "DAY" | "WEEK" | "MONTH" | "YEAR" | "OVERALL" | Unrecognized<string>
```