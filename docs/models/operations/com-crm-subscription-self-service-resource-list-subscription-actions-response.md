# ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsResponse

OK

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsResponse } from "crmcom/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsResponse = {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
      hasMore: true,
    },
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        code: "8047448052702285",
        executedOn: 1583846865,
        scheduledOn: 1583846865,
        cancelledOn: 1583846865,
        rejectedOn: 1583846865,
        category: {
          id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
          name: "Universal Name",
        },
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                       | Type                                                                                                                                                                                        | Required                                                                                                                                                                                    | Description                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                    | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsPaging](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-actions-paging.md)     | :heavy_minus_sign:                                                                                                                                                                          | N/A                                                                                                                                                                                         |
| `content`                                                                                                                                                                                   | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionActionsContent](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-actions-content.md)[] | :heavy_minus_sign:                                                                                                                                                                          | N/A                                                                                                                                                                                         |