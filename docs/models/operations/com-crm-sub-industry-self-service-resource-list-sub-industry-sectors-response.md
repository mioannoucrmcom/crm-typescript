# ComCrmSubIndustrySelfServiceResourceListSubIndustrySectorsResponse

OK

## Example Usage

```typescript
import { ComCrmSubIndustrySelfServiceResourceListSubIndustrySectorsResponse } from "crmcom/models/operations";

let value: ComCrmSubIndustrySelfServiceResourceListSubIndustrySectorsResponse =
  {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
    },
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "oil",
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                     | Type                                                                                                                                                                                      | Required                                                                                                                                                                                  | Description                                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                  | [operations.ComCrmSubIndustrySelfServiceResourceListSubIndustrySectorsPaging](../../models/operations/com-crm-sub-industry-self-service-resource-list-sub-industry-sectors-paging.md)     | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |
| `content`                                                                                                                                                                                 | [operations.ComCrmSubIndustrySelfServiceResourceListSubIndustrySectorsContent](../../models/operations/com-crm-sub-industry-self-service-resource-list-sub-industry-sectors-content.md)[] | :heavy_minus_sign:                                                                                                                                                                        | N/A                                                                                                                                                                                       |