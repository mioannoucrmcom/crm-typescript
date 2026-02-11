# ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesOrganisation

Details about the organisation (w/ creatives) that performed such customer event

## Example Usage

```typescript
import { ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesOrganisation } from "crm/models/operations";

let value:
  ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesOrganisation = {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "CRMdotCOM Nicosia",
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

| Field                                                                                                                                                                                                                 | Type                                                                                                                                                                                                                  | Required                                                                                                                                                                                                              | Description                                                                                                                                                                                                           | Example                                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                                                  | *string*                                                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                                    | The entity identifier                                                                                                                                                                                                 | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                                  |
| `name`                                                                                                                                                                                                                | *string*                                                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                                    | The organisation name                                                                                                                                                                                                 | CRMdotCOM Nicosia                                                                                                                                                                                                     |
| `creatives`                                                                                                                                                                                                           | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesOrganisationCreative](../../models/operations/com-crm-purchase-customer-event-self-service-resource-list-purchases-organisation-creative.md)[] | :heavy_minus_sign:                                                                                                                                                                                                    | A creative is an object that contains all the data required for visually rendering an image responsively. The object contains the initial image and a number of scale versions of it (srcset)                         |                                                                                                                                                                                                                       |