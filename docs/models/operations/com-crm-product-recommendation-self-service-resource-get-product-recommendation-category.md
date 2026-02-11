# ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationCategory

## Example Usage

```typescript
import { ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationCategory } from "crmcom/models/operations";

let value:
  ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationCategory =
    {
      type: "BEST_SELLING",
      id: "bestsellingproductsid",
      name: "Best selling products",
      description: "These are the best selling products in a month period",
      validityEnds: 1590474228,
      products: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          sku: "P0000101",
          name: "Base TV",
          description: "Basic TV & myFlix",
          pricing: [
            {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              price: 9.99,
              label: "9.99",
              currencyCode: "EUR",
              isDefault: true,
              taxModel: "TAX_INCLUSIVE",
              priceModel: "FLAT",
              supplyMethod: "DELIVERY",
              salesModel: {
                id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
                name: "Universal Name",
              },
              orderQueue: {
                id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
                name: "Universal Name",
              },
              priceTerms: {
                billingPeriod: {
                  duration: 2,
                  uot: "MONTH",
                },
                trialPeriod: {
                  duration: 2,
                  uot: "YEAR",
                },
                accessPeriod: {
                  startDate: 1612953199,
                  endDate: 1612953199,
                },
                billingModel: "PRE_BILL",
                contractPeriod: {
                  duration: 2,
                  uot: "HOUR",
                },
                rentalService: {
                  id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
                  name: "Universal Name",
                  sku: "S0001",
                },
                valueType: "VARIABLE",
              },
              tiers: [
                {
                  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
                  lowerTier: 1,
                  upperTier: 5,
                  price: 8.99,
                },
              ],
            },
          ],
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
      hasMore: true,
    };
```

## Fields

| Field                                                                                                                                                                                                            | Type                                                                                                                                                                                                             | Required                                                                                                                                                                                                         | Description                                                                                                                                                                                                      | Example                                                                                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                                                                                                                                                                                                           | [operations.ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationType](../../models/operations/com-crm-product-recommendation-self-service-resource-get-product-recommendation-type.md)         | :heavy_minus_sign:                                                                                                                                                                                               | The category type                                                                                                                                                                                                | BEST_SELLING                                                                                                                                                                                                     |
| `id`                                                                                                                                                                                                             | *string*                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                               | The category id                                                                                                                                                                                                  | bestsellingproductsid                                                                                                                                                                                            |
| `name`                                                                                                                                                                                                           | *string*                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                               | The category name                                                                                                                                                                                                | Best selling products                                                                                                                                                                                            |
| `description`                                                                                                                                                                                                    | *string*                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                               | The category description                                                                                                                                                                                         | These are the best selling products in a month period                                                                                                                                                            |
| `validityEnds`                                                                                                                                                                                                   | *number*                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                               | The date that the category expires (applicable for REWARD_OFFER_PROMOTION category type)                                                                                                                         | 1590474228                                                                                                                                                                                                       |
| `products`                                                                                                                                                                                                       | [operations.ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationProduct](../../models/operations/com-crm-product-recommendation-self-service-resource-get-product-recommendation-product.md)[] | :heavy_minus_sign:                                                                                                                                                                                               | The products that belong to the specified category                                                                                                                                                               |                                                                                                                                                                                                                  |
| `hasMore`                                                                                                                                                                                                        | *boolean*                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                               | If more products exist                                                                                                                                                                                           | true                                                                                                                                                                                                             |