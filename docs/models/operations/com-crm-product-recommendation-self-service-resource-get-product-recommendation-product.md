# ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationProduct

## Example Usage

```typescript
import { ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationProduct } from "crmcom/models/operations";

let value:
  ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationProduct =
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
              url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
            },
          ],
        },
      ],
    };
```

## Fields

| Field                                                                                                                                                                                                              | Type                                                                                                                                                                                                               | Required                                                                                                                                                                                                           | Description                                                                                                                                                                                                        | Example                                                                                                                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                                                               | *string*                                                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                                 | The product’s id                                                                                                                                                                                                   | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                               |
| `sku`                                                                                                                                                                                                              | *string*                                                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                                 | The product’s SKU                                                                                                                                                                                                  | P0000101                                                                                                                                                                                                           |
| `name`                                                                                                                                                                                                             | *string*                                                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                                 | Product name                                                                                                                                                                                                       | Base TV                                                                                                                                                                                                            |
| `description`                                                                                                                                                                                                      | *string*                                                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                                 | Product description                                                                                                                                                                                                | Basic TV & myFlix                                                                                                                                                                                                  |
| `pricing`                                                                                                                                                                                                          | [operations.ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationPricing](../../models/operations/com-crm-product-recommendation-self-service-resource-get-product-recommendation-pricing.md)[]   | :heavy_minus_sign:                                                                                                                                                                                                 | Product's pricing information                                                                                                                                                                                      |                                                                                                                                                                                                                    |
| `creatives`                                                                                                                                                                                                        | [operations.ComCrmProductRecommendationSelfServiceResourceGetProductRecommendationCreative](../../models/operations/com-crm-product-recommendation-self-service-resource-get-product-recommendation-creative.md)[] | :heavy_minus_sign:                                                                                                                                                                                                 | Details about creatives. A creative is an object that contains all the data required for visually rendering an image responsively, such as the initial image and a number of scale versions of it (srcset)         |                                                                                                                                                                                                                    |