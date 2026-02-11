# ComCrmEstimateOrderSelfServiceResourceEstimateOrderComponentsChange

## Example Usage

```typescript
import { ComCrmEstimateOrderSelfServiceResourceEstimateOrderComponentsChange } from "crm/models/operations";

let value: ComCrmEstimateOrderSelfServiceResourceEstimateOrderComponentsChange =
  {
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

| Field                                                                                                                                                                                          | Type                                                                                                                                                                                           | Required                                                                                                                                                                                       | Description                                                                                                                                                                                    |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `service`                                                                                                                                                                                      | [operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderService](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-service.md)                        | :heavy_minus_sign:                                                                                                                                                                             | N/A                                                                                                                                                                                            |
| `componentsAdded`                                                                                                                                                                              | [operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderComponentsAdded](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-components-added.md)[]     | :heavy_minus_sign:                                                                                                                                                                             | N/A                                                                                                                                                                                            |
| `componentsRemoved`                                                                                                                                                                            | [operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderComponentsRemoved](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-components-removed.md)[] | :heavy_minus_sign:                                                                                                                                                                             | N/A                                                                                                                                                                                            |