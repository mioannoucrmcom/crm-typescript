# OrderServicesToAddState

Service's State

## Example Usage

```typescript
import { OrderServicesToAddState } from "crmcom/models/operations";

let value: OrderServicesToAddState = "EFFECTIVE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"DRAFT" | "EFFECTIVE" | "NOT_EFFECTIVE" | "PAUSED" | "REGRETTED" | "CANCELLED" | "SWAPPED" | "REMOVED" | Unrecognized<string>
```