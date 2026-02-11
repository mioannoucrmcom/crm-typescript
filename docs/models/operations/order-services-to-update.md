# OrderServicesToUpdate

## Example Usage

```typescript
import { OrderServicesToUpdate } from "crmcom/models/operations";

let value: OrderServicesToUpdate = {
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

| Field                                                                                                           | Type                                                                                                            | Required                                                                                                        | Description                                                                                                     | Example                                                                                                         |
| --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| `state`                                                                                                         | [operations.OrderServicesToUpdateState](../../models/operations/order-services-to-update-state.md)              | :heavy_minus_sign:                                                                                              | Service's State                                                                                                 | EFFECTIVE                                                                                                       |
| `product`                                                                                                       | [operations.OrderServicesToUpdateProduct](../../models/operations/order-services-to-update-product.md)          | :heavy_minus_sign:                                                                                              | N/A                                                                                                             |                                                                                                                 |
| `trialPeriod`                                                                                                   | [operations.OrderServicesToUpdateTrialPeriod](../../models/operations/order-services-to-update-trial-period.md) | :heavy_minus_sign:                                                                                              | N/A                                                                                                             |                                                                                                                 |
| `quantity`                                                                                                      | *number*                                                                                                        | :heavy_minus_sign:                                                                                              | N/A                                                                                                             | 5                                                                                                               |
| `dependencies`                                                                                                  | [operations.OrderServicesToUpdateDependency](../../models/operations/order-services-to-update-dependency.md)[]  | :heavy_minus_sign:                                                                                              | N/A                                                                                                             |                                                                                                                 |
| `components`                                                                                                    | [operations.OrderServicesToUpdateComponent](../../models/operations/order-services-to-update-component.md)[]    | :heavy_minus_sign:                                                                                              | N/A                                                                                                             |                                                                                                                 |