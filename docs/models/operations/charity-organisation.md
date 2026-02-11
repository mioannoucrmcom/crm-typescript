# CharityOrganisation

Details about the organisation that such reward offer is donating to

## Example Usage

```typescript
import { CharityOrganisation } from "crmcom/models/operations";

let value: CharityOrganisation = {
  id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
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
};
```

## Fields

| Field                                                                                                                                                                                         | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   | Example                                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                          | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The organisation identifier                                                                                                                                                                   | 34b059a3-2aa7-b2c2-4191-a966168e97d7                                                                                                                                                          |
| `name`                                                                                                                                                                                        | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The organisation name                                                                                                                                                                         | Universal Name                                                                                                                                                                                |
| `creatives`                                                                                                                                                                                   | [operations.CharityOrganisationCreative](../../models/operations/charity-organisation-creative.md)[]                                                                                          | :heavy_minus_sign:                                                                                                                                                                            | A creative is an object that contains all the data required for visually rendering an image responsively. The object contains the initial image and a number of scale versions of it (srcset) |                                                                                                                                                                                               |