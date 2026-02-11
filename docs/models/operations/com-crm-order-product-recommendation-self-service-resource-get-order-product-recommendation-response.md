# ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationResponse

OK

## Example Usage

```typescript
import {
  ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationResponse,
} from "crmcom/models/operations";

let value:
  ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationResponse =
    {
      crossSells: [
        {
          pricing: {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
            currencyCode: "EUR",
            taxModel: "TAX_INCLUSIVE",
            tiers: {
              upperTier: 1,
              numberOfTiers: 3,
            },
            billingPeriod: {
              duration: 2,
              uot: "WEEK",
            },
            measurementUnit: {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              name: "Gigabytes",
              displayName: "GB",
            },
            accessPeriod: {
              startDate: 1612953199,
              endDate: 1612953199,
            },
            orderQueue: {
              id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
              name: "Universal Name",
            },
          },
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
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
                },
              ],
            },
          ],
        },
      ],
      upsells: [
        {
          pricing: {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
            currencyCode: "EUR",
            taxModel: "TAX_INCLUSIVE",
            tiers: {
              upperTier: 1,
              numberOfTiers: 3,
            },
            billingPeriod: {
              duration: 2,
              uot: "MONTH",
            },
            measurementUnit: {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              name: "Gigabytes",
              displayName: "GB",
            },
            accessPeriod: {
              startDate: 1612953199,
              endDate: 1612953199,
            },
            orderQueue: {
              id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
              name: "Universal Name",
            },
          },
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
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
                },
              ],
            },
          ],
        },
      ],
      rewardOffers: [
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
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
                },
              ],
            },
          ],
        },
      ],
      promotions: [
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
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
                },
              ],
            },
          ],
        },
      ],
    };
```

## Fields

| Field                                                                                                                                                                                                                                           | Type                                                                                                                                                                                                                                            | Required                                                                                                                                                                                                                                        | Description                                                                                                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `crossSells`                                                                                                                                                                                                                                    | [operations.ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationCrossSell](../../models/operations/com-crm-order-product-recommendation-self-service-resource-get-order-product-recommendation-cross-sell.md)[]     | :heavy_minus_sign:                                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                                             |
| `upsells`                                                                                                                                                                                                                                       | [operations.ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationUpsell](../../models/operations/com-crm-order-product-recommendation-self-service-resource-get-order-product-recommendation-upsell.md)[]            | :heavy_minus_sign:                                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                                             |
| `rewardOffers`                                                                                                                                                                                                                                  | [operations.ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationRewardOffer](../../models/operations/com-crm-order-product-recommendation-self-service-resource-get-order-product-recommendation-reward-offer.md)[] | :heavy_minus_sign:                                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                                             |
| `promotions`                                                                                                                                                                                                                                    | [operations.ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationPromotion](../../models/operations/com-crm-order-product-recommendation-self-service-resource-get-order-product-recommendation-promotion.md)[]      | :heavy_minus_sign:                                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                                             |