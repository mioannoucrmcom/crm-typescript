# CrossSellUot

Period Cycle unit of time

## Example Usage

```typescript
import { CrossSellUot } from "crm/models/operations";

let value: CrossSellUot = "MINUTE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SECOND" | "MINUTE" | "HOUR" | "DAY" | "WEEK" | "MONTH" | "YEAR" | "OVERALL" | Unrecognized<string>
```