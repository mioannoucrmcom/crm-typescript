# PeriodUot

The period’s unit of time

## Example Usage

```typescript
import { PeriodUot } from "crm/models/operations";

let value: PeriodUot = "MONTH";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SECOND" | "MINUTE" | "HOUR" | "DAY" | "WEEK" | "MONTH" | "YEAR" | "OVERALL" | Unrecognized<string>
```