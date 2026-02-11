# GetContactPreferredOrganisationSSResponse

OK

## Example Usage

```typescript
import { GetContactPreferredOrganisationSSResponse } from "crmcom/models/operations";

let value: GetContactPreferredOrganisationSSResponse = {
  organisations: [
    {
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
    },
  ],
};
```

## Fields

| Field                                                                                                                                       | Type                                                                                                                                        | Required                                                                                                                                    | Description                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| `organisations`                                                                                                                             | [operations.GetContactPreferredOrganisationSSOrganisation](../../models/operations/get-contact-preferred-organisation-ss-organisation.md)[] | :heavy_minus_sign:                                                                                                                          | N/A                                                                                                                                         |