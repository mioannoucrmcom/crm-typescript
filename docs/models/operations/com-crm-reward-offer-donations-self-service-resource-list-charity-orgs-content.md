# ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsContent

## Example Usage

```typescript
import { ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsContent } from "crm/models/operations";

let value: ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsContent =
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
            url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
          },
        ],
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                                      | Type                                                                                                                                                                                                       | Required                                                                                                                                                                                                   | Description                                                                                                                                                                                                | Example                                                                                                                                                                                                    |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                                       | *string*                                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                         | The entity identifier                                                                                                                                                                                      | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                       |
| `name`                                                                                                                                                                                                     | *string*                                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                         | The organisation name                                                                                                                                                                                      | 10% off any purchase                                                                                                                                                                                       |
| `description`                                                                                                                                                                                              | *string*                                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                         | The organisation description                                                                                                                                                                               | Donation Short Description                                                                                                                                                                                 |
| `creatives`                                                                                                                                                                                                | [operations.ComCrmRewardOfferDonationsSelfServiceResourceListCharityOrgsCreative](../../models/operations/com-crm-reward-offer-donations-self-service-resource-list-charity-orgs-creative.md)[]            | :heavy_minus_sign:                                                                                                                                                                                         | Details about creatives. A creative is an object that contains all the data required for visually rendering an image responsively, such as the initial image and a number of scale versions of it (srcset) |                                                                                                                                                                                                            |