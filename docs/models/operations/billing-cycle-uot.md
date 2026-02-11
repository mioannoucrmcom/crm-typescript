# BillingCycleUot

Billing cycle unit of time

## Example Usage

```typescript
import { BillingCycleUot } from "crm/models/operations";

let value: BillingCycleUot = "DAY";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SECOND" | "MINUTE" | "HOUR" | "DAY" | "WEEK" | "MONTH" | "YEAR" | "OVERALL" | Unrecognized<string>
```