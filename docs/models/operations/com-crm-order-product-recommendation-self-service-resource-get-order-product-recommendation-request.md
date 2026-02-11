# ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationRequest

## Example Usage

```typescript
import {
  ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationRequest,
} from "crm/models/operations";

let value:
  ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationRequest =
    {
      estimationId: "<id>",
      includeCreatives: true,
      includeCrossSells: true,
      includePromotions: true,
      includeRewardOffers: true,
      includeUpsells: true,
    };
```

## Fields

| Field                                                               | Type                                                                | Required                                                            | Description                                                         | Example                                                             |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `estimationId`                                                      | *string*                                                            | :heavy_check_mark:                                                  | Recommend products based on what is included in an order estimation |                                                                     |
| `includeCreatives`                                                  | *boolean*                                                           | :heavy_minus_sign:                                                  | Include recommended products creatives                              | true                                                                |
| `includeCrossSells`                                                 | *boolean*                                                           | :heavy_minus_sign:                                                  | Include cross-sell products in the recommndation                    | true                                                                |
| `includePromotions`                                                 | *boolean*                                                           | :heavy_minus_sign:                                                  | Include promotions in the recommndation                             | true                                                                |
| `includeRewardOffers`                                               | *boolean*                                                           | :heavy_minus_sign:                                                  | Include reward offers in the recommndation                          | true                                                                |
| `includeUpsells`                                                    | *boolean*                                                           | :heavy_minus_sign:                                                  | Include up-sell products in the recommndation                       | true                                                                |
| `orderCatalogueIds`                                                 | *string*                                                            | :heavy_minus_sign:                                                  | Recommend products based on order catalogues                        |                                                                     |