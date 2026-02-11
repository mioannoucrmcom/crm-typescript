# OrderServicesToChange

## Example Usage

```typescript
import { OrderServicesToChange } from "crm/models/operations";

let value: OrderServicesToChange = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  state: "EFFECTIVE",
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
  changeToProduct: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
};
```

## Fields

| Field                                                                                                          | Type                                                                                                           | Required                                                                                                       | Description                                                                                                    | Example                                                                                                        |
| -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                           | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | The entity identifier                                                                                          | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                           |
| `state`                                                                                                        | [operations.OrderServicesToChangeState](../../models/operations/order-services-to-change-state.md)             | :heavy_minus_sign:                                                                                             | Service's State                                                                                                | EFFECTIVE                                                                                                      |
| `product`                                                                                                      | [operations.OrderServicesToChangeProduct](../../models/operations/order-services-to-change-product.md)         | :heavy_minus_sign:                                                                                             | N/A                                                                                                            |                                                                                                                |
| `changeToProduct`                                                                                              | [operations.OrderChangeToProduct](../../models/operations/order-change-to-product.md)                          | :heavy_minus_sign:                                                                                             | N/A                                                                                                            |                                                                                                                |
| `quantity`                                                                                                     | *number*                                                                                                       | :heavy_minus_sign:                                                                                             | N/A                                                                                                            |                                                                                                                |
| `dependencies`                                                                                                 | [operations.OrderServicesToChangeDependency](../../models/operations/order-services-to-change-dependency.md)[] | :heavy_minus_sign:                                                                                             | N/A                                                                                                            |                                                                                                                |