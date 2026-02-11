# ComCrmContactSelfServiceResourceListContactDonationsResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceListContactDonationsResponse } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceListContactDonationsResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
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
                url:
                  "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
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
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                       | Type                                                                                                                                                                        | Required                                                                                                                                                                    | Description                                                                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                    | [operations.ComCrmContactSelfServiceResourceListContactDonationsPaging](../../models/operations/com-crm-contact-self-service-resource-list-contact-donations-paging.md)     | :heavy_minus_sign:                                                                                                                                                          | N/A                                                                                                                                                                         |
| `content`                                                                                                                                                                   | [operations.ComCrmContactSelfServiceResourceListContactDonationsContent](../../models/operations/com-crm-contact-self-service-resource-list-contact-donations-content.md)[] | :heavy_minus_sign:                                                                                                                                                          | N/A                                                                                                                                                                         |