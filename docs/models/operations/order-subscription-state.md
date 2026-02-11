# OrderSubscriptionState

## Example Usage

```typescript
import { OrderSubscriptionState } from "crm/models/operations";

let value: OrderSubscriptionState = "ACTIVE";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"ACTIVE" | "CHURNED" | "INACTIVE" | Unrecognized<string>
```