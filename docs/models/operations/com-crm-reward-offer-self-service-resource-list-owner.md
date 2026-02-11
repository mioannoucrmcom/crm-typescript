# ComCrmRewardOfferSelfServiceResourceListOwner

Details about organisation (w/ creatives)

## Example Usage

```typescript
import { ComCrmRewardOfferSelfServiceResourceListOwner } from "crm/models/operations";

let value: ComCrmRewardOfferSelfServiceResourceListOwner = {
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
};
```

## Fields

| Field                                                                                                                                                                                         | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   | Example                                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                          | *any*                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                            | The organisation identifier                                                                                                                                                                   | e66d45b4-2673-0a0e-5a06-d6088a324b3f                                                                                                                                                          |
| `name`                                                                                                                                                                                        | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The organisation name                                                                                                                                                                         | Pizza Yummy                                                                                                                                                                                   |
| `creatives`                                                                                                                                                                                   | [operations.ComCrmRewardOfferSelfServiceResourceListOwnerCreative](../../models/operations/com-crm-reward-offer-self-service-resource-list-owner-creative.md)[]                               | :heavy_minus_sign:                                                                                                                                                                            | A creative is an object that contains all the data required for visually rendering an image responsively. The object contains the initial image and a number of scale versions of it (srcset) |                                                                                                                                                                                               |