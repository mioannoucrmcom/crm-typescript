# ComCrmContactSelfServiceResourceGetOrganisationsResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetOrganisationsResponse } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceGetOrganisationsResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "BrewCoffee",
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
      wallet: {
        walletId: "038af54e-282c-40ad-ae5d-cc74f2c80f40",
        balance: 9.99,
        currencyCode: "EUR",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                              | Type                                                                                                                                                               | Required                                                                                                                                                           | Description                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `paging`                                                                                                                                                           | [operations.ComCrmContactSelfServiceResourceGetOrganisationsPaging](../../models/operations/com-crm-contact-self-service-resource-get-organisations-paging.md)     | :heavy_minus_sign:                                                                                                                                                 | N/A                                                                                                                                                                |
| `content`                                                                                                                                                          | [operations.ComCrmContactSelfServiceResourceGetOrganisationsContent](../../models/operations/com-crm-contact-self-service-resource-get-organisations-content.md)[] | :heavy_minus_sign:                                                                                                                                                 | N/A                                                                                                                                                                |