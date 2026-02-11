# ConditionProduct

The product that should be included in the basket

## Example Usage

```typescript
import { ConditionProduct } from "crm/models/operations";

let value: ConditionProduct = {
  itemType: "SKU",
  itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
  sku: "HDSTB123",
  name: "HD STB",
};
```

## Fields

| Field                                                                          | Type                                                                           | Required                                                                       | Description                                                                    | Example                                                                        |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| `itemType`                                                                     | [operations.ConditionItemType](../../models/operations/condition-item-type.md) | :heavy_check_mark:                                                             | The type of the product condition                                              | SKU                                                                            |
| `itemId`                                                                       | *string*                                                                       | :heavy_check_mark:                                                             | The identifier of the product/type/brand/family.                               | 4dc0809f-ed91-4b68-b912-5bd6064d901e                                           |
| `sku`                                                                          | *string*                                                                       | :heavy_minus_sign:                                                             | The product’s SKU. Applicable only when item type is set to Product            | HDSTB123                                                                       |
| `name`                                                                         | *string*                                                                       | :heavy_minus_sign:                                                             | The name of the product/type/brand/family                                      | HD STB                                                                         |