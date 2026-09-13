# BillingStateResponse

The usage records's billing state, i.e. if it was charged or not.

## Example Usage

```typescript
import { BillingStateResponse } from "crm/models/operations";

let value: BillingStateResponse = "PENDING";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"PENDING" | "COMPLETED" | Unrecognized<string>
```