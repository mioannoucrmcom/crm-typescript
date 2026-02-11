# ComCrmPromotionSelfServiceResourceGetSingleResponse

OK

## Example Usage

```typescript
import { ComCrmPromotionSelfServiceResourceGetSingleResponse } from "crm/models/operations";

let value: ComCrmPromotionSelfServiceResourceGetSingleResponse = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Sales season",
  state: "ACTIVE",
  shortDescription: "£10 off",
  longDescription: "£10 off on products whose price is more than £100",
  availability: {
    fromDate: 1648067185,
    toDate: 1648067185,
  },
  targets: {
    contact: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Universal Name",
    },
    segments: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "VIP contacts",
        description: "The VIP contacts",
        size: 10,
      },
    ],
    organisations: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "Good Burgers",
        type: "MERCHANT",
      },
    ],
    timings: {
      fixedPeriod: {
        startDate: 1648067185,
        endDate: 1648067185,
      },
      availability: null,
    },
  },
  basket: {
    products: {
      groups: [
        {
          group: "G1",
          operator: "AND",
          conditions: [
            {
              operator: "OR",
              product: {
                itemType: "SKU",
                itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
                sku: "HDSTB123",
                name: "HD STB",
              },
              quantity: 1,
              value: 9.99,
              billingCycle: {
                duration: 1,
                uot: "DAY",
              },
              contractPeriod: {
                duration: 12,
                uot: "MONTH",
              },
              services: [
                {
                  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
                  sku: "TV001",
                  name: "Films",
                  quantity: 2,
                },
              ],
            },
          ],
        },
      ],
    },
    rules: [
      {
        supplyMethods: [
          "DELIVERY",
        ],
        value: 9.99,
        quantity: 5,
      },
    ],
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
  offerings: [
    {
      product: {
        itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
        name: "HD STB",
        sku: "STB12345",
      },
      amount: 1.99,
      duration: {
        type: "PERIOD",
        period: {
          duration: 6,
          uot: "MONTH",
        },
        variableDiscounts: [
          {
            type: "PERCENT",
            amount: 1.99,
            period: {
              duration: 6,
              uot: "MONTH",
            },
            periodOrder: 1,
          },
        ],
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                         | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   | Example                                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                          | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The entity identifier                                                                                                                                                                         | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                          |
| `name`                                                                                                                                                                                        | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | Promotion name                                                                                                                                                                                | Sales season                                                                                                                                                                                  |
| `state`                                                                                                                                                                                       | [operations.ComCrmPromotionSelfServiceResourceGetSingleState](../../models/operations/com-crm-promotion-self-service-resource-get-single-state.md)                                            | :heavy_minus_sign:                                                                                                                                                                            | Promotion state                                                                                                                                                                               | ACTIVE                                                                                                                                                                                        |
| `shortDescription`                                                                                                                                                                            | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | Short description of the Promotion                                                                                                                                                            | £10 off                                                                                                                                                                                       |
| `longDescription`                                                                                                                                                                             | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | A more detailed description of the Promotion                                                                                                                                                  | £10 off on products whose price is more than £100                                                                                                                                             |
| `availability`                                                                                                                                                                                | [operations.ComCrmPromotionSelfServiceResourceGetSingleAvailability](../../models/operations/com-crm-promotion-self-service-resource-get-single-availability.md)                              | :heavy_minus_sign:                                                                                                                                                                            | Determines when the Promotion is available and will be applied. A Promotion is applied only when purchases are performed within this period.                                                  |                                                                                                                                                                                               |
| `targets`                                                                                                                                                                                     | [operations.ComCrmPromotionSelfServiceResourceGetSingleTargets](../../models/operations/com-crm-promotion-self-service-resource-get-single-targets.md)                                        | :heavy_minus_sign:                                                                                                                                                                            | The Promotion’s target conditions i.e. the required conditions for the contact to get the discount.                                                                                           |                                                                                                                                                                                               |
| `basket`                                                                                                                                                                                      | [operations.Basket](../../models/operations/basket.md)                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                            | N/A                                                                                                                                                                                           |                                                                                                                                                                                               |
| `creatives`                                                                                                                                                                                   | [operations.ComCrmPromotionSelfServiceResourceGetSingleCreative](../../models/operations/com-crm-promotion-self-service-resource-get-single-creative.md)[]                                    | :heavy_minus_sign:                                                                                                                                                                            | A creative is an object that contains all the data required for visually rendering an image responsively. The object contains the initial image and a number of scale versions of it (srcset) |                                                                                                                                                                                               |
| `offerings`                                                                                                                                                                                   | [operations.Offering](../../models/operations/offering.md)[]                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                            | N/A                                                                                                                                                                                           |                                                                                                                                                                                               |