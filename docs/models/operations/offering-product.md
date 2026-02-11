# OfferingProduct

The product on which the discount will be applied

## Example Usage

```typescript
import { OfferingProduct } from "crmcom/models/operations";

let value: OfferingProduct = {
  itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
  name: "HD STB",
  sku: "STB12345",
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  | Example                                                                      |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `itemId`                                                                     | *string*                                                                     | :heavy_minus_sign:                                                           | The unique identifier of the product item                                    | 4dc0809f-ed91-4b68-b912-5bd6064d901e                                         |
| `itemType`                                                                   | [operations.OfferingItemType](../../models/operations/offering-item-type.md) | :heavy_minus_sign:                                                           | Determines on which product the discount will be applied.                    |                                                                              |
| `name`                                                                       | *string*                                                                     | :heavy_minus_sign:                                                           | The product/type/brand/family name                                           | HD STB                                                                       |
| `sku`                                                                        | *string*                                                                     | :heavy_minus_sign:                                                           | The product’s SKU. Applicable only for SKU item types                        | STB12345                                                                     |