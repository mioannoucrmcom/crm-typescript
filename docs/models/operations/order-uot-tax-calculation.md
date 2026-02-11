# OrderUotTaxCalculation

The billing cycle's unit of time

## Example Usage

```typescript
import { OrderUotTaxCalculation } from "crmcom/models/operations";

let value: OrderUotTaxCalculation = "MONTH";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SECOND" | "MINUTE" | "HOUR" | "DAY" | "WEEK" | "MONTH" | "YEAR" | "OVERALL" | Unrecognized<string>
```