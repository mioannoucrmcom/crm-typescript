# ComCrmMerchantSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmMerchantSelfServiceResourceListResponse } from "crmcom/models/operations";

let value: ComCrmMerchantSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "CRMdotCOM",
      description: "The best rewards company",
    },
  ],
};
```

## Fields

| Field                                                                                                                                       | Type                                                                                                                                        | Required                                                                                                                                    | Description                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                    | [operations.ComCrmMerchantSelfServiceResourceListPaging](../../models/operations/com-crm-merchant-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                          | N/A                                                                                                                                         |
| `content`                                                                                                                                   | [operations.ComCrmMerchantSelfServiceResourceListContent](../../models/operations/com-crm-merchant-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                          | N/A                                                                                                                                         |