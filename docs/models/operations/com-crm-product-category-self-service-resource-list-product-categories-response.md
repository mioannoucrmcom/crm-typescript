# ComCrmProductCategorySelfServiceResourceListProductCategoriesResponse

OK

## Example Usage

```typescript
import { ComCrmProductCategorySelfServiceResourceListProductCategoriesResponse } from "crmcom/models/operations";

let value:
  ComCrmProductCategorySelfServiceResourceListProductCategoriesResponse = {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
      hasMore: true,
    },
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "Milk Options Cappuccino",
        displayName: "Milk Option",
        code: "Milks01",
        description: "Milk Options for Cappuccino",
        childNodes: 2,
        parent: {
          id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
          name: "Universal Name",
        },
        availableInOrderMenus: false,
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
                url:
                  "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
              },
            ],
          },
        ],
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                          | Type                                                                                                                                                                                           | Required                                                                                                                                                                                       | Description                                                                                                                                                                                    |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                       | [operations.ComCrmProductCategorySelfServiceResourceListProductCategoriesPaging](../../models/operations/com-crm-product-category-self-service-resource-list-product-categories-paging.md)     | :heavy_minus_sign:                                                                                                                                                                             | N/A                                                                                                                                                                                            |
| `content`                                                                                                                                                                                      | [operations.ComCrmProductCategorySelfServiceResourceListProductCategoriesContent](../../models/operations/com-crm-product-category-self-service-resource-list-product-categories-content.md)[] | :heavy_minus_sign:                                                                                                                                                                             | N/A                                                                                                                                                                                            |