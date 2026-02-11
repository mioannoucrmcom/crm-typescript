# AuthorisedUsageService

## Example Usage

```typescript
import { AuthorisedUsageService } from "crm/models/operations";

let value: AuthorisedUsageService = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  classification: "TRACEABLE_PHYSICAL_GOOD",
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
};
```

## Fields

| Field                                                                                                   | Type                                                                                                    | Required                                                                                                | Description                                                                                             | Example                                                                                                 |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                    | *string*                                                                                                | :heavy_minus_sign:                                                                                      | The entity identifier                                                                                   | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                    |
| `classification`                                                                                        | [operations.AuthorisedUsageClassification](../../models/operations/authorised-usage-classification.md)  | :heavy_minus_sign:                                                                                      | Product type classification                                                                             | TRACEABLE_PHYSICAL_GOOD                                                                                 |
| `product`                                                                                               | [operations.AuthorisedUsageServiceProduct](../../models/operations/authorised-usage-service-product.md) | :heavy_minus_sign:                                                                                      | N/A                                                                                                     |                                                                                                         |