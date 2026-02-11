# OrderDevicesAdded

## Example Usage

```typescript
import { OrderDevicesAdded } from "crm/models/operations";

let value: OrderDevicesAdded = {
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `quantity`                                                                                    | *number*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `product`                                                                                     | [operations.OrderDevicesAddedProduct](../../models/operations/order-devices-added-product.md) | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `serialNumber`                                                                                | *string*[]                                                                                    | :heavy_minus_sign:                                                                            | N/A                                                                                           |