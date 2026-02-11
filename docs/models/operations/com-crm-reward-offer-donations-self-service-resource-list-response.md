# ComCrmRewardOfferDonationsSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmRewardOfferDonationsSelfServiceResourceListResponse } from "crmcom/models/operations";

let value: ComCrmRewardOfferDonationsSelfServiceResourceListResponse = {
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
      type: "ONE_OFF",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                 | Type                                                                                                                                                                  | Required                                                                                                                                                              | Description                                                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                              | [operations.ComCrmRewardOfferDonationsSelfServiceResourceListPaging](../../models/operations/com-crm-reward-offer-donations-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                                                    | N/A                                                                                                                                                                   |
| `content`                                                                                                                                                             | [operations.ComCrmRewardOfferDonationsSelfServiceResourceListContent](../../models/operations/com-crm-reward-offer-donations-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                                                    | N/A                                                                                                                                                                   |