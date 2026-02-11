# ComponentState

Component Service's State

## Example Usage

```typescript
import { ComponentState } from "crmcom/models/operations";

let value: ComponentState = "EFFECTIVE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"DRAFT" | "EFFECTIVE" | "NOT_EFFECTIVE" | "PAUSED" | "REGRETTED" | "CANCELLED" | "SWAPPED" | "REMOVED" | Unrecognized<string>
```