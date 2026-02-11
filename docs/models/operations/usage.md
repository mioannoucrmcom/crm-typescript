# Usage

## Example Usage

```typescript
import { Usage } from "crmcom/models/operations";

let value: Usage = {
  product: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    sku: "FREDESPR001",
  },
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `product`                                                                                  | [operations.ProductRequest](../../models/operations/product-request.md)                    | :heavy_minus_sign:                                                                         | The usage product to be consumed (either a usage service or a non-traceable physical good) |
| `usageAmount`                                                                              | *number*                                                                                   | :heavy_minus_sign:                                                                         | The usage amount to be consumed. Either usage amount or cash amount should be specified    |
| `cashAmount`                                                                               | *number*                                                                                   | :heavy_minus_sign:                                                                         | The cash amount to be consumed. Either usage amount or cash amount should be specified     |