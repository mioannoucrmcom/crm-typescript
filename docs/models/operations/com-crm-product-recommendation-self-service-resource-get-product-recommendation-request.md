# ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationRequest

## Example Usage

```typescript
import { ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationRequest } from "crm/models/operations";

let value:
  ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationRequest =
    {};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `categoryId`                                                                 | *string*                                                                     | :heavy_minus_sign:                                                           | The category identifier.                                                     |
| `categoryType`                                                               | [operations.CategoryType](../../models/operations/category-type.md)          | :heavy_minus_sign:                                                           | The category type.                                                           |
| `contactId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | The contact identifier. Either a contact or an orgnaisation can be specified |
| `size`                                                                       | *number*                                                                     | :heavy_minus_sign:                                                           | The amount of products we want to get for each category                      |