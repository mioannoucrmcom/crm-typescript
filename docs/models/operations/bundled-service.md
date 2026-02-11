# BundledService

Applicable when the service was added as part of a bundled service

## Example Usage

```typescript
import { BundledService } from "crm/models/operations";

let value: BundledService = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            | Example                                                                                |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `id`                                                                                   | *string*                                                                               | :heavy_minus_sign:                                                                     | The entity identifier                                                                  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                   |
| `product`                                                                              | [operations.BundledServiceProduct](../../models/operations/bundled-service-product.md) | :heavy_minus_sign:                                                                     | Bundle service product                                                                 |                                                                                        |