# ComCrmApprovalRequestSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmApprovalRequestSelfServiceResourceListResponse } from "crm/models/operations";

let value: ComCrmApprovalRequestSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      entity: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        reference: "O10214",
        stageId: "O10214",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                      | Type                                                                                                                                                       | Required                                                                                                                                                   | Description                                                                                                                                                |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                   | [operations.ComCrmApprovalRequestSelfServiceResourceListPaging](../../models/operations/com-crm-approval-request-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                                         | N/A                                                                                                                                                        |
| `content`                                                                                                                                                  | [operations.ComCrmApprovalRequestSelfServiceResourceListContent](../../models/operations/com-crm-approval-request-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                                         | N/A                                                                                                                                                        |