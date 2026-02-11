# ComCrmRewardOfferSelfServiceResourceGetSingleResponse

OK

## Example Usage

```typescript
import { ComCrmRewardOfferSelfServiceResourceGetSingleResponse } from "crmcom/models/operations";

let value: ComCrmRewardOfferSelfServiceResourceGetSingleResponse = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "10% off any purchase",
  shortDescription: "Short Description",
  longDescription: "Long Description",
  termsAndConditions: "Terms & Conditions",
  availability: {
    from: 1606819297,
    to: 1606819297,
  },
  isFeatured: false,
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
            url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
          },
        ],
      },
    ],
  },
  performanceEnabled: true,
  scheme: {
    id: "58a54215-5d8f-5b40-af91-c62e86b973a9",
    name: "Loyalty Scheme",
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
  targets: {
    organisations: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "Bravo Bakery",
        locations: [
          {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
            name: "Head Office",
            addressLine1: "Elia Papakyriakou 21",
            addressLine2: "7 Tower Stars",
            stateProvinceCounty: "Egkomi",
            townCity: "Nicosia",
            postalCode: "2415",
            countryCode: "CYP",
            careOf: "c/o Company",
            lat: 35.157115,
            lon: 35.342115,
            googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
            isPrimary: true,
            isBilling: true,
            isTestMode: true,
          },
        ],
        type: "MERCHANT",
      },
    ],
  },
};
```

## Fields

| Field                                                                                                                                                                                                                                                                | Type                                                                                                                                                                                                                                                                 | Required                                                                                                                                                                                                                                                             | Description                                                                                                                                                                                                                                                          | Example                                                                                                                                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                                                                                                 | *string*                                                                                                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                                                                                   | The entity identifier                                                                                                                                                                                                                                                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                                                                                 |
| `name`                                                                                                                                                                                                                                                               | *string*                                                                                                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                                                                                   | The reward offer name                                                                                                                                                                                                                                                | 10% off any purchase                                                                                                                                                                                                                                                 |
| `shortDescription`                                                                                                                                                                                                                                                   | *string*                                                                                                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                                                                                   | The reward offer short description                                                                                                                                                                                                                                   | Short Description                                                                                                                                                                                                                                                    |
| `longDescription`                                                                                                                                                                                                                                                    | *string*                                                                                                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                                                                                   | The reward offer long description                                                                                                                                                                                                                                    | Long Description                                                                                                                                                                                                                                                     |
| `termsAndConditions`                                                                                                                                                                                                                                                 | *string*                                                                                                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                                                                                                   | The reward offer terms and conditions                                                                                                                                                                                                                                | Terms & Conditions                                                                                                                                                                                                                                                   |
| `availability`                                                                                                                                                                                                                                                       | [operations.ComCrmRewardOfferSelfServiceResourceGetSingleAvailability](../../models/operations/com-crm-reward-offer-self-service-resource-get-single-availability.md)                                                                                                | :heavy_minus_sign:                                                                                                                                                                                                                                                   | The offer availability (from-to) dates (whithin this period customers will be awarded)                                                                                                                                                                               |                                                                                                                                                                                                                                                                      |
| `isFeatured`                                                                                                                                                                                                                                                         | *boolean*                                                                                                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                                                                                                   | Defines whether the reward offer is set as featured                                                                                                                                                                                                                  | false                                                                                                                                                                                                                                                                |
| `owner`                                                                                                                                                                                                                                                              | [operations.ComCrmRewardOfferSelfServiceResourceGetSingleOwner](../../models/operations/com-crm-reward-offer-self-service-resource-get-single-owner.md)                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                                                                                   | Details about organisation (w/ creatives)                                                                                                                                                                                                                            |                                                                                                                                                                                                                                                                      |
| `performanceEnabled`                                                                                                                                                                                                                                                 | *boolean*                                                                                                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                                                                                                   | Defines whether the reward offer is eligible to be used for performance purposes (e.g. for every 100 euros worth of goods, get 10 euros back). Performance based offers have a completion target and usually is presented in the form of a percentage line or stamps | true                                                                                                                                                                                                                                                                 |
| `scheme`                                                                                                                                                                                                                                                             | [operations.ComCrmRewardOfferSelfServiceResourceGetSingleScheme](../../models/operations/com-crm-reward-offer-self-service-resource-get-single-scheme.md)                                                                                                            | :heavy_minus_sign:                                                                                                                                                                                                                                                   | Details about reward scheme                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                                      |
| `creatives`                                                                                                                                                                                                                                                          | [operations.ComCrmRewardOfferSelfServiceResourceGetSingleCreative](../../models/operations/com-crm-reward-offer-self-service-resource-get-single-creative.md)[]                                                                                                      | :heavy_minus_sign:                                                                                                                                                                                                                                                   | A creative is an object that contains all the data required for visually rendering an image responsively. The object contains the initial image and a number of scale versions of it (srcset)                                                                        |                                                                                                                                                                                                                                                                      |
| `targets`                                                                                                                                                                                                                                                            | [operations.ComCrmRewardOfferSelfServiceResourceGetSingleTargets](../../models/operations/com-crm-reward-offer-self-service-resource-get-single-targets.md)                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                                                                                   | The targerted organisations that events performed on should be located at                                                                                                                                                                                            |                                                                                                                                                                                                                                                                      |