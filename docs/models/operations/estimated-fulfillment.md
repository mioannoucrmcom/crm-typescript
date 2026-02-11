# EstimatedFulfillment

When the order is estimated to be fulfilled

## Example Usage

```typescript
import { EstimatedFulfillment } from "crmcom/models/operations";

let value: EstimatedFulfillment = {
  date: 1592809457,
  duration: 30,
  uot: "MINUTE",
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                | Example                                                                                    |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `date`                                                                                     | *number*                                                                                   | :heavy_minus_sign:                                                                         | The actual date on which the order will be fulfilled                                       | 1592809457                                                                                 |
| `duration`                                                                                 | *number*                                                                                   | :heavy_minus_sign:                                                                         | How much time to fufill                                                                    | 30                                                                                         |
| `uot`                                                                                      | [operations.EstimatedFulfillmentUot](../../models/operations/estimated-fulfillment-uot.md) | :heavy_minus_sign:                                                                         | Unit of time to fulfilled time                                                             | MINUTE                                                                                     |