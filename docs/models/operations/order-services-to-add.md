# OrderServicesToAdd

## Example Usage

```typescript
import { OrderServicesToAdd } from "crm/models/operations";

let value: OrderServicesToAdd = {
  state: "EFFECTIVE",
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
  trialPeriod: {
    startsOn: 12345678,
    endsOn: 12345678,
  },
  quantity: 5,
  components: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      quantity: 5,
    },
  ],
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               | Example                                                                                                   |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `state`                                                                                                   | [operations.OrderServicesToAddState](../../models/operations/order-services-to-add-state.md)              | :heavy_minus_sign:                                                                                        | Service's State                                                                                           | EFFECTIVE                                                                                                 |
| `product`                                                                                                 | [operations.OrderServicesToAddProduct](../../models/operations/order-services-to-add-product.md)          | :heavy_minus_sign:                                                                                        | N/A                                                                                                       |                                                                                                           |
| `trialPeriod`                                                                                             | [operations.OrderServicesToAddTrialPeriod](../../models/operations/order-services-to-add-trial-period.md) | :heavy_minus_sign:                                                                                        | N/A                                                                                                       |                                                                                                           |
| `quantity`                                                                                                | *number*                                                                                                  | :heavy_minus_sign:                                                                                        | N/A                                                                                                       | 5                                                                                                         |
| `dependencies`                                                                                            | [operations.OrderServicesToAddDependency](../../models/operations/order-services-to-add-dependency.md)[]  | :heavy_minus_sign:                                                                                        | N/A                                                                                                       |                                                                                                           |
| `components`                                                                                              | [operations.OrderServicesToAddComponent](../../models/operations/order-services-to-add-component.md)[]    | :heavy_minus_sign:                                                                                        | N/A                                                                                                       |                                                                                                           |