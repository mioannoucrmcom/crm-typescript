# ComCrmQueueSelfServiceResourceListContent

## Example Usage

```typescript
import { ComCrmQueueSelfServiceResourceListContent } from "crmcom/models/operations";

let value: ComCrmQueueSelfServiceResourceListContent = {
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
};
```

## Fields

| Field                                                                                                                                   | Type                                                                                                                                    | Required                                                                                                                                | Description                                                                                                                             | Example                                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                    | *string*                                                                                                                                | :heavy_minus_sign:                                                                                                                      | The entity identifier                                                                                                                   | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                    |
| `name`                                                                                                                                  | *string*                                                                                                                                | :heavy_minus_sign:                                                                                                                      | The queue’s name                                                                                                                        | Billing Issues                                                                                                                          |
| `classification`                                                                                                                        | *string*                                                                                                                                | :heavy_minus_sign:                                                                                                                      | The queue’s classification                                                                                                              |                                                                                                                                         |
| `owner`                                                                                                                                 | [operations.ComCrmQueueSelfServiceResourceListOwner](../../models/operations/com-crm-queue-self-service-resource-list-owner.md)         | :heavy_minus_sign:                                                                                                                      | The queue’s owner                                                                                                                       |                                                                                                                                         |
| `defaultPriority`                                                                                                                       | [operations.DefaultPriority](../../models/operations/default-priority.md)                                                               | :heavy_minus_sign:                                                                                                                      | The queue’s default priority                                                                                                            |                                                                                                                                         |
| `defaultTags`                                                                                                                           | [operations.DefaultTag](../../models/operations/default-tag.md)[]                                                                       | :heavy_minus_sign:                                                                                                                      | The queue’s tags                                                                                                                        |                                                                                                                                         |
| `categories`                                                                                                                            | [operations.ComCrmQueueSelfServiceResourceListCategory](../../models/operations/com-crm-queue-self-service-resource-list-category.md)[] | :heavy_minus_sign:                                                                                                                      | The queue’s categories                                                                                                                  |                                                                                                                                         |