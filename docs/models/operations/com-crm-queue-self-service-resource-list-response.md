# ComCrmQueueSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmQueueSelfServiceResourceListResponse } from "crmcom/models/operations";

let value: ComCrmQueueSelfServiceResourceListResponse = {
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Billing Issues",
      owner: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
      },
      defaultPriority: {
        urgency: "MEDIUM",
        impact: "MEDIUM",
        priority: "MEDIUM",
      },
      defaultTags: [
        {
          tagId: "JKGJHFSDJHGDSJHGA",
          name: "Maintenance",
        },
      ],
      categories: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "Physical Maintenance",
          description: "General Maintenance issues.",
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                 | Type                                                                                                                                  | Required                                                                                                                              | Description                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| `content`                                                                                                                             | [operations.ComCrmQueueSelfServiceResourceListContent](../../models/operations/com-crm-queue-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                    | N/A                                                                                                                                   |