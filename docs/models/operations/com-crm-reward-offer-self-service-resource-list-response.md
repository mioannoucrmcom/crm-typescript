# ComCrmRewardOfferSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmRewardOfferSelfServiceResourceListResponse } from "crmcom/models/operations";

let value: ComCrmRewardOfferSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "10% off any purchase",
      scheme: {
        id: "58a54215-5d8f-5b40-af91-c62e86b973a9",
        name: "Loyalty Scheme",
      },
      shortDescription: "Short Description",
      longDescription: "Long Description",
      termsAndConditions: "Terms & Conditions",
      goal: "ACHIEVEMENT",
      type: "LOTTERY",
      owner: {
        id: "e66d45b4-2673-0a0e-5a06-d6088a324b3f",
        name: "Pizza Yummy",
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
      isFeatured: false,
      performanceEnabled: true,
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
    },
  ],
};
```

## Fields

| Field                                                                                                                                              | Type                                                                                                                                               | Required                                                                                                                                           | Description                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                           | [operations.ComCrmRewardOfferSelfServiceResourceListPaging](../../models/operations/com-crm-reward-offer-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                                 | N/A                                                                                                                                                |
| `content`                                                                                                                                          | [operations.ComCrmRewardOfferSelfServiceResourceListContent](../../models/operations/com-crm-reward-offer-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                                 | N/A                                                                                                                                                |