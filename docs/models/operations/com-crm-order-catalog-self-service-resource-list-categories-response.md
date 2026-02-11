# ComCrmOrderCatalogSelfServiceResourceListCategoriesResponse

OK

## Example Usage

```typescript
import { ComCrmOrderCatalogSelfServiceResourceListCategoriesResponse } from "crmcom/models/operations";

let value: ComCrmOrderCatalogSelfServiceResourceListCategoriesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Food",
      code: "FOOD",
      description: "Food",
      childNodes: 2,
      priority: 1,
      parent: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
      },
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
      products: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          product: {
            id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
            name: "Universal Name",
            sku: "S0001",
          },
          priority: 2,
        },
      ],
      billingPeriod: 5,
      billingPeriodUot: "MINUTE",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                     | Type                                                                                                                                                                      | Required                                                                                                                                                                  | Description                                                                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                  | [operations.ComCrmOrderCatalogSelfServiceResourceListCategoriesPaging](../../models/operations/com-crm-order-catalog-self-service-resource-list-categories-paging.md)     | :heavy_minus_sign:                                                                                                                                                        | N/A                                                                                                                                                                       |
| `content`                                                                                                                                                                 | [operations.ComCrmOrderCatalogSelfServiceResourceListCategoriesContent](../../models/operations/com-crm-order-catalog-self-service-resource-list-categories-content.md)[] | :heavy_minus_sign:                                                                                                                                                        | N/A                                                                                                                                                                       |