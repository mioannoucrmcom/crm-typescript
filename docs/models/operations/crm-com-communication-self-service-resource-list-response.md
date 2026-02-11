# CrmComCommunicationSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { CrmComCommunicationSelfServiceResourceListResponse } from "crmcom/models/operations";

let value: CrmComCommunicationSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Happy Birthday",
      isViewed: false,
      viewedOn: 1583846865,
      isArchived: true,
      clickedOn: 1583846865,
      createdOn: 1583846865,
      language: "ENG",
      sender: "dev@crm.com",
      recipient: "jon@crm.com",
      subtitle: "20% discount for December",
      subject: "Welcome to our company",
      content: "Dear sir/madam...",
      contact: {
        id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
        name: "John Smith",
        code: "H8893M70",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                 | Type                                                                                                                                                  | Required                                                                                                                                              | Description                                                                                                                                           |
| ----------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                              | [operations.CrmComCommunicationSelfServiceResourceListPaging](../../models/operations/crm-com-communication-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                                    | N/A                                                                                                                                                   |
| `content`                                                                                                                                             | [operations.CrmComCommunicationSelfServiceResourceListContent](../../models/operations/crm-com-communication-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                                    | N/A                                                                                                                                                   |