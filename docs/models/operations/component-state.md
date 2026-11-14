# ComponentState

Component Service's State

## Example Usage

```typescript
import { ComponentState } from "crm/models/operations";

let value: ComponentState = "EFFECTIVE";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"DRAFT" | "EFFECTIVE" | "NOT_EFFECTIVE" | "PAUSED" | "REGRETTED" | "CANCELLED" | "SWAPPED" | "REMOVED" | Unrecognized<string>
```