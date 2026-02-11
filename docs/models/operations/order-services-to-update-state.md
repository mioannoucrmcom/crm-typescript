# OrderServicesToUpdateState

Service's State

## Example Usage

```typescript
import { OrderServicesToUpdateState } from "crm/models/operations";

let value: OrderServicesToUpdateState = "EFFECTIVE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"DRAFT" | "EFFECTIVE" | "NOT_EFFECTIVE" | "PAUSED" | "REGRETTED" | "CANCELLED" | "SWAPPED" | "REMOVED" | Unrecognized<string>
```