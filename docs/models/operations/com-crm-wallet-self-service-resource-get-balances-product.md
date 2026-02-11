# ComCrmWalletSelfServiceResourceGetBalancesProduct

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetBalancesProduct } from "crm/models/operations";

let value: ComCrmWalletSelfServiceResourceGetBalancesProduct = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Coffee",
  description: "Brazilian Coffee",
  sku: "COF-5541",
};
```

## Fields

| Field                                                   | Type                                                    | Required                                                | Description                                             | Example                                                 |
| ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- |
| `id`                                                    | *string*                                                | :heavy_minus_sign:                                      | The entity identifier                                   | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                    |
| `idType`                                                | [operations.IdType](../../models/operations/id-type.md) | :heavy_minus_sign:                                      | The type of the ID to be provided                       |                                                         |
| `name`                                                  | *string*                                                | :heavy_minus_sign:                                      | The name of the product                                 | Coffee                                                  |
| `description`                                           | *string*                                                | :heavy_minus_sign:                                      | The description of the product                          | Brazilian Coffee                                        |
| `sku`                                                   | *string*                                                | :heavy_minus_sign:                                      | The product sku                                         | COF-5541                                                |