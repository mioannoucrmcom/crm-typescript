# ComCrmIndustrySelfServiceResourceListIndustriesResponse

OK

## Example Usage

```typescript
import { ComCrmIndustrySelfServiceResourceListIndustriesResponse } from "crmcom/models/operations";

let value: ComCrmIndustrySelfServiceResourceListIndustriesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "gas",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                            | Type                                                                                                                                                             | Required                                                                                                                                                         | Description                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                         | [operations.ComCrmIndustrySelfServiceResourceListIndustriesPaging](../../models/operations/com-crm-industry-self-service-resource-list-industries-paging.md)     | :heavy_minus_sign:                                                                                                                                               | N/A                                                                                                                                                              |
| `content`                                                                                                                                                        | [operations.ComCrmIndustrySelfServiceResourceListIndustriesContent](../../models/operations/com-crm-industry-self-service-resource-list-industries-content.md)[] | :heavy_minus_sign:                                                                                                                                               | N/A                                                                                                                                                              |