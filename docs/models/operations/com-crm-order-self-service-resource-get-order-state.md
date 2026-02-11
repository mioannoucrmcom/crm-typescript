# ComCrmOrderSelfServiceResourceGetOrderState

The order’s life cycle state

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceGetOrderState } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourceGetOrderState = "COMPLETED";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"NEW" | "IN_PROGRESS" | "COMPLETED" | "CANCELLED" | "ON_HOLD" | Unrecognized<string>
```