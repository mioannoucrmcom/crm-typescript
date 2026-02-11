# ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionComponentsChange

## Example Usage

```typescript
import {
  ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionComponentsChange,
} from "crm/models/operations";

let value:
  ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionComponentsChange =
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

| Field                                                                                                                                                                                                                      | Type                                                                                                                                                                                                                       | Required                                                                                                                                                                                                                   | Description                                                                                                                                                                                                                |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `service`                                                                                                                                                                                                                  | [operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionService](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-subscription-service.md)                        | :heavy_minus_sign:                                                                                                                                                                                                         | N/A                                                                                                                                                                                                                        |
| `componentsAdded`                                                                                                                                                                                                          | [operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionComponentsAdded](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-subscription-components-added.md)[]     | :heavy_minus_sign:                                                                                                                                                                                                         | N/A                                                                                                                                                                                                                        |
| `componentsRemoved`                                                                                                                                                                                                        | [operations.ComCrmEstimateSubscriptionSelfServiceResourceEstimateSubscriptionComponentsRemoved](../../models/operations/com-crm-estimate-subscription-self-service-resource-estimate-subscription-components-removed.md)[] | :heavy_minus_sign:                                                                                                                                                                                                         | N/A                                                                                                                                                                                                                        |