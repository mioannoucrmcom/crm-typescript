# RelatedTermedService

Applicable only when the device is enabled on a one-time service which extends a termed service

## Example Usage

```typescript
import { RelatedTermedService } from "crm/models/operations";

let value: RelatedTermedService = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         | Example                                                                                             |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `id`                                                                                                | *string*                                                                                            | :heavy_minus_sign:                                                                                  | The entity identifier                                                                               | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                |
| `product`                                                                                           | [operations.RelatedTermedServiceProduct](../../models/operations/related-termed-service-product.md) | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |                                                                                                     |