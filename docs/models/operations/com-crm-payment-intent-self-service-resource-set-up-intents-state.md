# ComCrmPaymentIntentSelfServiceResourceSetUpIntentsState

The payment intent state

## Example Usage

```typescript
import { ComCrmPaymentIntentSelfServiceResourceSetUpIntentsState } from "crm/models/operations";

let value: ComCrmPaymentIntentSelfServiceResourceSetUpIntentsState = "PENDING";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"REQUIRES_CAPTURING" | "REJECTED" | "COMPLETED" | "PENDING" | "CANCELLED" | Unrecognized<string>
```