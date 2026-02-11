# ComCrmServiceRequestSelfServiceResourceGetNotesResponse

OK

## Example Usage

```typescript
import { ComCrmServiceRequestSelfServiceResourceGetNotesResponse } from "crmcom/models/operations";

let value: ComCrmServiceRequestSelfServiceResourceGetNotesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      createdOn: 98765775,
      updatedOn: 98765775,
      createdBy: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        username: "Sam Jackson",
        name: "S_Jackson",
      },
      pinned: true,
      note:
        "After my telephone conversation with Zack this morning, it was decided that....",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                             | Type                                                                                                                                                              | Required                                                                                                                                                          | Description                                                                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                          | [operations.ComCrmServiceRequestSelfServiceResourceGetNotesPaging](../../models/operations/com-crm-service-request-self-service-resource-get-notes-paging.md)     | :heavy_minus_sign:                                                                                                                                                | N/A                                                                                                                                                               |
| `content`                                                                                                                                                         | [operations.ComCrmServiceRequestSelfServiceResourceGetNotesContent](../../models/operations/com-crm-service-request-self-service-resource-get-notes-content.md)[] | :heavy_minus_sign:                                                                                                                                                | N/A                                                                                                                                                               |