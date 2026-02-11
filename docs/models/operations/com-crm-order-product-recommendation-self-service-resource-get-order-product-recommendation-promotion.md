# ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationPromotion

## Example Usage

```typescript
import {
  ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationPromotion,
} from "crmcom/models/operations";

let value:
  ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationPromotion =
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      creatives: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          width: 2159,
          height: 3075,
          format: "jpg",
          url: "https://assets.crm.com/image/offer.jpg",
          publicId: "crm-com/image",
          media: [
            {
              width: 200,
              height: 300,
              url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
            },
          ],
        },
      ],
    };
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     | Example                                                                         |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `id`                                                                            | *string*                                                                        | :heavy_minus_sign:                                                              | The entity identifier                                                           | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                            |
| `name`                                                                          | *string*                                                                        | :heavy_minus_sign:                                                              | N/A                                                                             |                                                                                 |
| `creatives`                                                                     | [operations.PromotionCreative](../../models/operations/promotion-creative.md)[] | :heavy_minus_sign:                                                              | N/A                                                                             |                                                                                 |