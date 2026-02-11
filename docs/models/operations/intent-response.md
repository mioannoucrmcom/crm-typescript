# IntentResponse

The intent for which the token was requested

## Example Usage

```typescript
import { IntentResponse } from "crm/models/operations";

let value: IntentResponse = "SPEND";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"APPROVE_PURCHASE" | "REJECT_PURCHASE" | "SPEND" | Unrecognized<string>
```