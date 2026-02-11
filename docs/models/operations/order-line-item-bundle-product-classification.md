# OrderLineItemBundleProductClassification

Product type classification

## Example Usage

```typescript
import { OrderLineItemBundleProductClassification } from "crmcom/models/operations";

let value: OrderLineItemBundleProductClassification = "TRACEABLE_PHYSICAL_GOOD";
```

## Values

This is an open enum. Unrecognized values will be captured as the `Unrecognized<string>` branded type.

```typescript
"TERMED_SERVICE" | "USAGE_SERVICE" | "ONE_TIME_SERVICE" | "TRACEABLE_PHYSICAL_GOOD" | "NON_TRACEABLE_PHYSICAL_GOOD" | "EXPENSES_SERVICE" | Unrecognized<string>
```