# ConditionContractPeriodUot

Contract period unit of time

## Example Usage

```typescript
import { ConditionContractPeriodUot } from "crm/models/operations";

let value: ConditionContractPeriodUot = "MONTH";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SECOND" | "MINUTE" | "HOUR" | "DAY" | "WEEK" | "MONTH" | "YEAR" | "OVERALL" | Unrecognized<string>
```