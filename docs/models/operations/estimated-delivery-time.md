# EstimatedDeliveryTime

An estimation of the delivery time

## Example Usage

```typescript
import { EstimatedDeliveryTime } from "crmcom/models/operations";

let value: EstimatedDeliveryTime = {
  timeToDelivery: 20,
  uot: "MINUTE",
  deliveryAt: 1599224678,
};
```

## Fields

| Field                                                                                                                                      | Type                                                                                                                                       | Required                                                                                                                                   | Description                                                                                                                                | Example                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `timeToDelivery`                                                                                                                           | *number*                                                                                                                                   | :heavy_minus_sign:                                                                                                                         | N/A                                                                                                                                        | 20                                                                                                                                         |
| `uot`                                                                                                                                      | [operations.ComCrmOrderSelfServiceResourceCreateOrderUot](../../models/operations/com-crm-order-self-service-resource-create-order-uot.md) | :heavy_minus_sign:                                                                                                                         | N/A                                                                                                                                        | MINUTE                                                                                                                                     |
| `deliveryAt`                                                                                                                               | *number*                                                                                                                                   | :heavy_minus_sign:                                                                                                                         | The actual delivery time                                                                                                                   | 1599224678                                                                                                                                 |