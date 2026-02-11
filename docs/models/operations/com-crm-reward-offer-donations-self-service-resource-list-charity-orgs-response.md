# ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsResponse

OK

## Example Usage

```typescript
import { ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsResponse } from "crm/models/operations";

let value:
  ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsResponse = {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "10% off any purchase",
        description: "Donation Short Description",
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

| Field                                                                                                                                                                                         | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   | Example                                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                          | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The entity identifier                                                                                                                                                                         | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                          |
| `content`                                                                                                                                                                                     | [operations.ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsContent](../../models/operations/com-crm-reward-offer-donations-self-service-resource-list-charity-orgs-content.md)[] | :heavy_minus_sign:                                                                                                                                                                            | N/A                                                                                                                                                                                           |                                                                                                                                                                                               |