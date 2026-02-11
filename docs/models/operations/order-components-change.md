# OrderComponentsChange

## Example Usage

```typescript
import { OrderComponentsChange } from "crm/models/operations";

let value: OrderComponentsChange = {
  service: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
  componentsAdded: [
    {
      id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
      name: "Universal Name",
      sku: "S0001",
    },
  ],
  componentsRemoved: [
    {
      id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
      name: "Universal Name",
      sku: "S0001",
    },
  ],
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `service`                                                                                  | [operations.OrderService](../../models/operations/order-service.md)                        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `componentsAdded`                                                                          | [operations.OrderComponentsAdded](../../models/operations/order-components-added.md)[]     | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `componentsRemoved`                                                                        | [operations.OrderComponentsRemoved](../../models/operations/order-components-removed.md)[] | :heavy_minus_sign:                                                                         | N/A                                                                                        |