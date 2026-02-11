# AuthorisedUsage

## Example Usage

```typescript
import { AuthorisedUsage } from "crmcom/models/operations";

let value: AuthorisedUsage = {
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
  measurementUnit: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  },
  services: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      classification: "TRACEABLE_PHYSICAL_GOOD",
      product: {
        id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
        name: "Universal Name",
        sku: "S0001",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `amount`                                                                                                  | *number*                                                                                                  | :heavy_minus_sign:                                                                                        | N/A                                                                                                       |
| `usage`                                                                                                   | *number*                                                                                                  | :heavy_minus_sign:                                                                                        | N/A                                                                                                       |
| `product`                                                                                                 | [operations.AuthorisedUsageProduct](../../models/operations/authorised-usage-product.md)                  | :heavy_minus_sign:                                                                                        | The usage product to be consumed. Can either be a usage service or a non-traceable physical goods         |
| `measurementUnit`                                                                                         | [operations.AuthorisedUsageMeasurementUnit](../../models/operations/authorised-usage-measurement-unit.md) | :heavy_minus_sign:                                                                                        | The usage service's measurement unit                                                                      |
| `services`                                                                                                | [operations.AuthorisedUsageService](../../models/operations/authorised-usage-service.md)[]                | :heavy_minus_sign:                                                                                        | Unique list of services that provide usage allowance to the contact                                       |