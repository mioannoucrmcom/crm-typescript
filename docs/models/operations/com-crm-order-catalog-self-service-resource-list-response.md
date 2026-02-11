# ComCrmOrderCatalogSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmOrderCatalogSelfServiceResourceListResponse } from "crm/models/operations";

let value: ComCrmOrderCatalogSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Monday menu",
      description: "A list of dishes available every Monday",
      displayName: "Monday",
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
      supplyMethods: [
        "DELIVERY",
      ],
      timeAvailability: [
        {
          startTime: "09:00",
          endTime: "17:00",
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                                | Type                                                                                                                                                 | Required                                                                                                                                             | Description                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                             | [operations.ComCrmOrderCatalogSelfServiceResourceListPaging](../../models/operations/com-crm-order-catalog-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                                   | N/A                                                                                                                                                  |
| `content`                                                                                                                                            | [operations.ComCrmOrderCatalogSelfServiceResourceListContent](../../models/operations/com-crm-order-catalog-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                                   | N/A                                                                                                                                                  |