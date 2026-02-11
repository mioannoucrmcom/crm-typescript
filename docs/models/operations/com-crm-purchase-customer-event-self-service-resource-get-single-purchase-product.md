# ComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchaseProduct

## Example Usage

```typescript
import { ComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchaseProduct } from "crmcom/models/operations";

let value:
  ComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchaseProduct = {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    productSku: {
      id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
      name: "Universal Name",
      sku: "S00012",
    },
    productFamily: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Universal Name",
    },
    quantity: 1,
    netAmount: 1.08,
    taxAmount: 0.51,
    totalAmount: 1.59,
  };
```

## Fields

| Field                                                                 | Type                                                                  | Required                                                              | Description                                                           | Example                                                               |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `id`                                                                  | *string*                                                              | :heavy_minus_sign:                                                    | The entity identifier                                                 | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                  |
| `productSku`                                                          | [operations.ProductSku](../../models/operations/product-sku.md)       | :heavy_minus_sign:                                                    | Details about product SKU                                             |                                                                       |
| `productFamily`                                                       | [operations.ProductFamily](../../models/operations/product-family.md) | :heavy_minus_sign:                                                    | Details about product family                                          |                                                                       |
| `quantity`                                                            | *number*                                                              | :heavy_minus_sign:                                                    | The quantity of the purchased product                                 | 1                                                                     |
| `netAmount`                                                           | *number*                                                              | :heavy_minus_sign:                                                    | The net amount of the purchased product                               | 1.08                                                                  |
| `taxAmount`                                                           | *number*                                                              | :heavy_minus_sign:                                                    | The tax amount of the purchased product                               | 0.51                                                                  |
| `totalAmount`                                                         | *number*                                                              | :heavy_minus_sign:                                                    | The total amount (net + tax) of the purchased product                 | 1.59                                                                  |