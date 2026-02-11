# ComCrmAccountSelfServiceResourceListAccountJournalsResponse

OK

## Example Usage

```typescript
import { ComCrmAccountSelfServiceResourceListAccountJournalsResponse } from "crmcom/models/operations";

let value: ComCrmAccountSelfServiceResourceListAccountJournalsResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      number: "INV123",
      entityId: "7156b6b0-ab00-46c8-8411-c515c20d4e19",
      issuedDate: 1232412,
      postedDate: 1232412,
      transactionType: "INVOICE",
      type: "CREDIT",
      currencyCode: "EUR",
      amount: 15,
      invoice: {
        dueDate: 1232412,
        overdueAmount: 15,
        unpaidAmount: 15,
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                     | Type                                                                                                                                                                      | Required                                                                                                                                                                  | Description                                                                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                  | [operations.ComCrmAccountSelfServiceResourceListAccountJournalsPaging](../../models/operations/com-crm-account-self-service-resource-list-account-journals-paging.md)     | :heavy_minus_sign:                                                                                                                                                        | N/A                                                                                                                                                                       |
| `content`                                                                                                                                                                 | [operations.ComCrmAccountSelfServiceResourceListAccountJournalsContent](../../models/operations/com-crm-account-self-service-resource-list-account-journals-content.md)[] | :heavy_minus_sign:                                                                                                                                                        | N/A                                                                                                                                                                       |