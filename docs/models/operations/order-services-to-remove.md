# OrderServicesToRemove

## Example Usage

```typescript
import { OrderServicesToRemove } from "crm/models/operations";

let value: OrderServicesToRemove = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  state: "EFFECTIVE",
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
};
```

## Fields

| Field                                                                                                  | Type                                                                                                   | Required                                                                                               | Description                                                                                            | Example                                                                                                |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                   | *string*                                                                                               | :heavy_minus_sign:                                                                                     | The entity identifier                                                                                  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                   |
| `state`                                                                                                | [operations.OrderServicesToRemoveState](../../models/operations/order-services-to-remove-state.md)     | :heavy_minus_sign:                                                                                     | Service's State                                                                                        | EFFECTIVE                                                                                              |
| `product`                                                                                              | [operations.OrderServicesToRemoveProduct](../../models/operations/order-services-to-remove-product.md) | :heavy_minus_sign:                                                                                     | N/A                                                                                                    |                                                                                                        |