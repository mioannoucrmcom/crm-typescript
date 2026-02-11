# ProductRequest

The usage product to be consumed (either a usage service or a non-traceable physical good)

## Example Usage

```typescript
import { ProductRequest } from "crm/models/operations";

let value: ProductRequest = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  sku: "FREDESPR001",
};
```

## Fields

| Field                                                          | Type                                                           | Required                                                       | Description                                                    | Example                                                        |
| -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
| `id`                                                           | *string*                                                       | :heavy_check_mark:                                             | The product id (product id and product sku are semi-optional)  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                           |
| `sku`                                                          | *string*                                                       | :heavy_check_mark:                                             | The product sku (product id and product sku are semi-optional) | FREDESPR001                                                    |