# UpsellUot

Period Cycle unit of time

## Example Usage

```typescript
import { UpsellUot } from "crm/models/operations";

let value: UpsellUot = "WEEK";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SECOND" | "MINUTE" | "HOUR" | "DAY" | "WEEK" | "MONTH" | "YEAR" | "OVERALL" | Unrecognized<string>
```