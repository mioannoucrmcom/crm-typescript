# BillingPeriodUot

## Example Usage

```typescript
import { BillingPeriodUot } from "crm/models/operations";

let value: BillingPeriodUot = "MINUTE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SECOND" | "MINUTE" | "HOUR" | "DAY" | "WEEK" | "MONTH" | "YEAR" | "OVERALL" | Unrecognized<string>
```