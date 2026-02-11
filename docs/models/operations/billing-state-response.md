# BillingStateResponse

The usage records's billing state, i.e. if it was charged or not.

## Example Usage

```typescript
import { BillingStateResponse } from "crm/models/operations";

let value: BillingStateResponse = "PENDING";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"PENDING" | "COMPLETED" | Unrecognized<string>
```