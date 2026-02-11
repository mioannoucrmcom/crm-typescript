# OrderServicesToRemoveState

Service's State

## Example Usage

```typescript
import { OrderServicesToRemoveState } from "crmcom/models/operations";

let value: OrderServicesToRemoveState = "EFFECTIVE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"DRAFT" | "EFFECTIVE" | "NOT_EFFECTIVE" | "PAUSED" | "REGRETTED" | "CANCELLED" | "SWAPPED" | "REMOVED" | Unrecognized<string>
```