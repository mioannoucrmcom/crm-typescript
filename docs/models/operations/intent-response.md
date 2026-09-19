# IntentResponse

The intent for which the token was requested

## Example Usage

```typescript
import { IntentResponse } from "crm/models/operations";

let value: IntentResponse = "SPEND";

// Open enum: unrecognized values are captured as Unrecognized<string>
```

## Values

```typescript
"APPROVE_PURCHASE" | "REJECT_PURCHASE" | "SPEND" | Unrecognized<string>
```