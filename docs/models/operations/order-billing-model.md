# OrderBillingModel

## Example Usage

```typescript
import { OrderBillingModel } from "crmcom/models/operations";

let value: OrderBillingModel = "PRE_BILL";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"PRE_BILL" | "POST_BILL" | Unrecognized<string>
```