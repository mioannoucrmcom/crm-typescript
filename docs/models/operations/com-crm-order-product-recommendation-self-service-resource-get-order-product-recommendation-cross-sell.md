# ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationCrossSell

## Example Usage

```typescript
import {
  ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationCrossSell,
} from "crmcom/models/operations";

let value:
  ComCrmOrderProductRecommendationSelfServiceResourceGetOrderProductRecommendationCrossSell =
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
              url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
            },
          ],
        },
      ],
    };
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `id`                                                                             | *string*                                                                         | :heavy_minus_sign:                                                               | N/A                                                                              |
| `sku`                                                                            | *string*                                                                         | :heavy_minus_sign:                                                               | N/A                                                                              |
| `name`                                                                           | *string*                                                                         | :heavy_minus_sign:                                                               | N/A                                                                              |
| `description`                                                                    | *string*                                                                         | :heavy_minus_sign:                                                               | N/A                                                                              |
| `pricing`                                                                        | [operations.CrossSellPricing](../../models/operations/cross-sell-pricing.md)     | :heavy_minus_sign:                                                               | N/A                                                                              |
| `creatives`                                                                      | [operations.CrossSellCreative](../../models/operations/cross-sell-creative.md)[] | :heavy_minus_sign:                                                               | N/A                                                                              |