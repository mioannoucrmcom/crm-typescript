# ComCrmProductTypeSelfServiceResourceListProductTypesResponse

OK

## Example Usage

```typescript
import { ComCrmProductTypeSelfServiceResourceListProductTypesResponse } from "crmcom/models/operations";

let value: ComCrmProductTypeSelfServiceResourceListProductTypesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Decoders",
      displayName: "Decoders",
      description: "All Decoders",
      classification: "TERMED_SERVICE",
      compositionMethod: "FIXED_BUNDLE",
      taxCategory: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "Universal Name",
        code: "4134213343214141",
      },
      owner: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
      },
      characteristics: 3,
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                        | Type                                                                                                                                                                         | Required                                                                                                                                                                     | Description                                                                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                     | [operations.ComCrmProductTypeSelfServiceResourceListProductTypesPaging](../../models/operations/com-crm-product-type-self-service-resource-list-product-types-paging.md)     | :heavy_minus_sign:                                                                                                                                                           | N/A                                                                                                                                                                          |
| `content`                                                                                                                                                                    | [operations.ComCrmProductTypeSelfServiceResourceListProductTypesContent](../../models/operations/com-crm-product-type-self-service-resource-list-product-types-content.md)[] | :heavy_minus_sign:                                                                                                                                                           | N/A                                                                                                                                                                          |