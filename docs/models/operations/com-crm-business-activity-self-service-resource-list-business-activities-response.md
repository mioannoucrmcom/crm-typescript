# ComCrmBusinessActivitySelfServiceResourceListBusinessActivitiesResponse

OK

## Example Usage

```typescript
import { ComCrmBusinessActivitySelfServiceResourceListBusinessActivitiesResponse } from "crmcom/models/operations";

let value:
  ComCrmBusinessActivitySelfServiceResourceListBusinessActivitiesResponse = {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
    },
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "Bar & Grill",
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                              | Type                                                                                                                                                                                               | Required                                                                                                                                                                                           | Description                                                                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                           | [operations.ComCrmBusinessActivitySelfServiceResourceListBusinessActivitiesPaging](../../models/operations/com-crm-business-activity-self-service-resource-list-business-activities-paging.md)     | :heavy_minus_sign:                                                                                                                                                                                 | N/A                                                                                                                                                                                                |
| `content`                                                                                                                                                                                          | [operations.ComCrmBusinessActivitySelfServiceResourceListBusinessActivitiesContent](../../models/operations/com-crm-business-activity-self-service-resource-list-business-activities-content.md)[] | :heavy_minus_sign:                                                                                                                                                                                 | N/A                                                                                                                                                                                                |