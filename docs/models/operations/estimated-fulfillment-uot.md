# EstimatedFulfillmentUot

Unit of time to fulfilled time

## Example Usage

```typescript
import { EstimatedFulfillmentUot } from "crmcom/models/operations";

let value: EstimatedFulfillmentUot = "MINUTE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SECOND" | "MINUTE" | "HOUR" | "DAY" | "WEEK" | "MONTH" | "YEAR" | "OVERALL" | Unrecognized<string>
```