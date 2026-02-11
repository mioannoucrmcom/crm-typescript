# ComCrmProductSelfServiceResourceGetProductComponentsStockInformation

The product variant stock information (returned only if include_stock is set to true)

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductComponentsStockInformation } from "crmcom/models/operations";

let value:
  ComCrmProductSelfServiceResourceGetProductComponentsStockInformation = {
    stockBalance: 12,
    reserved: 1,
    inStock: true,
  };
```

## Fields

| Field                                                                   | Type                                                                    | Required                                                                | Description                                                             | Example                                                                 |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `stockBalance`                                                          | *number*                                                                | :heavy_minus_sign:                                                      | The number of items that are in the warehouse (including reserved ones) | 12                                                                      |
| `reserved`                                                              | *number*                                                                | :heavy_minus_sign:                                                      | The number of items that are reserved                                   | 1                                                                       |
| `inStock`                                                               | *boolean*                                                               | :heavy_minus_sign:                                                      | Applicable only for stockable physical goods                            | true                                                                    |