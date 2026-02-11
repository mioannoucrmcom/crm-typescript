# OrderEstimatedDelivery

## Example Usage

```typescript
import { OrderEstimatedDelivery } from "crm/models/operations";

let value: OrderEstimatedDelivery = {
  timeToDelivery: 1,
  uot: "MINUTE",
  deliveredAt: 12345565,
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             | Example                                                                                 |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `timeToDelivery`                                                                        | *number*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     | 1                                                                                       |
| `uot`                                                                                   | [operations.OrderOrderEstimateUot](../../models/operations/order-order-estimate-uot.md) | :heavy_minus_sign:                                                                      | N/A                                                                                     | MINUTE                                                                                  |
| `deliveredAt`                                                                           | *number*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     | 12345565                                                                                |