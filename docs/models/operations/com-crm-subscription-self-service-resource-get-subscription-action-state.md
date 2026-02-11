# ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionState

State of Subscription action

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionState } from "crm/models/operations";

let value: ComCrmSubscriptionSelfServiceResourceGetSubscriptionActionState =
  "CANCELLED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"SCHEDULED" | "EXECUTED" | "REJECTED" | "CANCELLED" | Unrecognized<string>
```