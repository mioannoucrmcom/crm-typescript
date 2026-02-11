# GetContactPreferredOrganisationSSOrganisation

## Example Usage

```typescript
import { GetContactPreferredOrganisationSSOrganisation } from "crm/models/operations";

let value: GetContactPreferredOrganisationSSOrganisation = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Down Town Burgers",
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

| Field                                                                                                                               | Type                                                                                                                                | Required                                                                                                                            | Description                                                                                                                         | Example                                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                | *string*                                                                                                                            | :heavy_minus_sign:                                                                                                                  | The entity identifier                                                                                                               | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                |
| `type`                                                                                                                              | [operations.GetContactPreferredOrganisationSSType](../../models/operations/get-contact-preferred-organisation-ss-type.md)           | :heavy_minus_sign:                                                                                                                  | The type of preferred organisation                                                                                                  |                                                                                                                                     |
| `name`                                                                                                                              | *string*                                                                                                                            | :heavy_minus_sign:                                                                                                                  | The organisation name                                                                                                               | Down Town Burgers                                                                                                                   |
| `creatives`                                                                                                                         | [operations.GetContactPreferredOrganisationSSCreative](../../models/operations/get-contact-preferred-organisation-ss-creative.md)[] | :heavy_minus_sign:                                                                                                                  | Creatives images for marketing includes the primary image and scaled versions to create a srcset                                    |                                                                                                                                     |