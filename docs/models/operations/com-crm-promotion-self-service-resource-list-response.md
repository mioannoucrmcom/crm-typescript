# ComCrmPromotionSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmPromotionSelfServiceResourceListResponse } from "crmcom/models/operations";

let value: ComCrmPromotionSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "20% Xmas",
      shortDescription: "20% off during Xmas time",
      longDescription:
        "20% off, unconditional avialable during Xmas time and up until the end of year",
      availability: {
        fromDate: 1648067185,
        toDate: 1648067185,
      },
      currencyCode: "EUR",
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
      tags: [
        {
          tagId: "JKGJHFSDJHGDSJHGA",
          name: "Maintenance",
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                         | Type                                                                                                                                          | Required                                                                                                                                      | Description                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                      | [operations.ComCrmPromotionSelfServiceResourceListPaging](../../models/operations/com-crm-promotion-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                            | N/A                                                                                                                                           |
| `content`                                                                                                                                     | [operations.ComCrmPromotionSelfServiceResourceListContent](../../models/operations/com-crm-promotion-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                            | N/A                                                                                                                                           |