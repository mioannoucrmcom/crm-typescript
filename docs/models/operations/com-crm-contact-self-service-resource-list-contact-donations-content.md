# ComCrmContactSelfServiceResourceListContactDonationsContent

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceListContactDonationsContent } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceListContactDonationsContent = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  optedIn: 1589796854,
  optedOut: 1589796854,
  donations: 12,
  amount: 40,
  currencyCode: "EUR",
  donationOffer: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
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
  organisation: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Universal Name",
  },
  details: {
    multiplier: 2,
    amount: 2,
  },
};
```

## Fields

| Field                                                                                                                                                                                  | Type                                                                                                                                                                                   | Required                                                                                                                                                                               | Description                                                                                                                                                                            | Example                                                                                                                                                                                |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                   | *string*                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                     | The entity identifier                                                                                                                                                                  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                   |
| `optedIn`                                                                                                                                                                              | *number*                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                     | The date on which the contact opted-in to the donation offers                                                                                                                          | 1589796854                                                                                                                                                                             |
| `optedOut`                                                                                                                                                                             | *number*                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                     | The date on which the contact opted-out from the donation offer.                                                                                                                       | 1589796854                                                                                                                                                                             |
| `donations`                                                                                                                                                                            | *number*                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                     | Number of donations made                                                                                                                                                               | 12                                                                                                                                                                                     |
| `amount`                                                                                                                                                                               | *number*                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                     | Total donated amount                                                                                                                                                                   | 40                                                                                                                                                                                     |
| `currencyCode`                                                                                                                                                                         | [operations.ComCrmContactSelfServiceResourceListContactDonationsCurrencyCode](../../models/operations/com-crm-contact-self-service-resource-list-contact-donations-currency-code.md)   | :heavy_minus_sign:                                                                                                                                                                     | The currency                                                                                                                                                                           | EUR                                                                                                                                                                                    |
| `donationOffer`                                                                                                                                                                        | [operations.ComCrmContactSelfServiceResourceListContactDonationsDonationOffer](../../models/operations/com-crm-contact-self-service-resource-list-contact-donations-donation-offer.md) | :heavy_minus_sign:                                                                                                                                                                     | The donation offer the contact is opt-in to.                                                                                                                                           |                                                                                                                                                                                        |
| `organisation`                                                                                                                                                                         | [operations.ComCrmContactSelfServiceResourceListContactDonationsOrganisation](../../models/operations/com-crm-contact-self-service-resource-list-contact-donations-organisation.md)    | :heavy_minus_sign:                                                                                                                                                                     | The organisation that receives the donation                                                                                                                                            |                                                                                                                                                                                        |
| `details`                                                                                                                                                                              | [operations.ComCrmContactSelfServiceResourceListContactDonationsDetails](../../models/operations/com-crm-contact-self-service-resource-list-contact-donations-details.md)              | :heavy_minus_sign:                                                                                                                                                                     | The donation's details that show how/when donations are made by the contact                                                                                                            |                                                                                                                                                                                        |