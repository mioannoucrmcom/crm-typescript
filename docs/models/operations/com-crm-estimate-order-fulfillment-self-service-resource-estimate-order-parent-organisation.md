# ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderParentOrganisation

Details about the parent organisation (business/merchant) of the fulfilled by. Not applicable if the fulfilled by organisation is of type business or merchant

## Example Usage

```typescript
import { ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderParentOrganisation } from "crmcom/models/operations";

let value:
  ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderParentOrganisation =
    {
      id: "b1607c37-e750-2324-ac49-6591a86f54b8",
      name: "Best Burger",
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

| Field                                                                                                                                                                                                                                    | Type                                                                                                                                                                                                                                     | Required                                                                                                                                                                                                                                 | Description                                                                                                                                                                                                                              | Example                                                                                                                                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                                                                     | *string*                                                                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                                                                       | The organisation identifier                                                                                                                                                                                                              | b1607c37-e750-2324-ac49-6591a86f54b8                                                                                                                                                                                                     |
| `name`                                                                                                                                                                                                                                   | *string*                                                                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                                                                       | The organisation name                                                                                                                                                                                                                    | Best Burger                                                                                                                                                                                                                              |
| `creatives`                                                                                                                                                                                                                              | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderParentOrganisationCreative](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-parent-organisation-creative.md)[] | :heavy_minus_sign:                                                                                                                                                                                                                       | Details about creatives. A creative is an object that contains all the data required for visually rendering an image responsively, such as the initial image and a number of scale versions of it (srcset)                               |                                                                                                                                                                                                                                          |