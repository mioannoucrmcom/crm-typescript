# ComCrmContactSelfServiceResourceGetOrganisationsContent

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetOrganisationsContent } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceGetOrganisationsContent = {
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
};
```

## Fields

| Field                                                                                                                                                                | Type                                                                                                                                                                 | Required                                                                                                                                                             | Description                                                                                                                                                          | Example                                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                 | *string*                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                   | The entity identifier                                                                                                                                                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                 |
| `name`                                                                                                                                                               | *string*                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                   | The organisation name                                                                                                                                                | BrewCoffee                                                                                                                                                           |
| `creatives`                                                                                                                                                          | [operations.ComCrmContactSelfServiceResourceGetOrganisationsCreative](../../models/operations/com-crm-contact-self-service-resource-get-organisations-creative.md)[] | :heavy_minus_sign:                                                                                                                                                   | Creatives images for marketing includes the primary image and scaled versions to create a srcset                                                                     |                                                                                                                                                                      |
| `wallet`                                                                                                                                                             | [operations.ComCrmContactSelfServiceResourceGetOrganisationsWallet](../../models/operations/com-crm-contact-self-service-resource-get-organisations-wallet.md)       | :heavy_minus_sign:                                                                                                                                                   | Contact wallet information for the organisation                                                                                                                      |                                                                                                                                                                      |