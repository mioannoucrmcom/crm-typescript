# ComCrmTagSelfServiceResourceListTagsResponse

OK

## Example Usage

```typescript
import { ComCrmTagSelfServiceResourceListTagsResponse } from "crm/models/operations";

let value: ComCrmTagSelfServiceResourceListTagsResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Maintenance",
      description: "This tag relates to maintenance issues",
      colour: "75FG77",
    },
  ],
};
```

## Fields

| Field                                                                                                                                      | Type                                                                                                                                       | Required                                                                                                                                   | Description                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `paging`                                                                                                                                   | [operations.ComCrmTagSelfServiceResourceListTagsPaging](../../models/operations/com-crm-tag-self-service-resource-list-tags-paging.md)     | :heavy_minus_sign:                                                                                                                         | N/A                                                                                                                                        |
| `content`                                                                                                                                  | [operations.ComCrmTagSelfServiceResourceListTagsContent](../../models/operations/com-crm-tag-self-service-resource-list-tags-content.md)[] | :heavy_minus_sign:                                                                                                                         | N/A                                                                                                                                        |