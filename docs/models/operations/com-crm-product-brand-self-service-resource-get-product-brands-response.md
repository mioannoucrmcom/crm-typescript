# ComCrmProductBrandSelfServiceResourceGetProductBrandsResponse

OK

## Example Usage

```typescript
import { ComCrmProductBrandSelfServiceResourceGetProductBrandsResponse } from "crmcom/models/operations";

let value: ComCrmProductBrandSelfServiceResourceGetProductBrandsResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "orange",
      description: "orange services",
      owner: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                          | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `paging`                                                                                                                                                                       | [operations.ComCrmProductBrandSelfServiceResourceGetProductBrandsPaging](../../models/operations/com-crm-product-brand-self-service-resource-get-product-brands-paging.md)     | :heavy_minus_sign:                                                                                                                                                             | N/A                                                                                                                                                                            |
| `content`                                                                                                                                                                      | [operations.ComCrmProductBrandSelfServiceResourceGetProductBrandsContent](../../models/operations/com-crm-product-brand-self-service-resource-get-product-brands-content.md)[] | :heavy_minus_sign:                                                                                                                                                             | N/A                                                                                                                                                                            |