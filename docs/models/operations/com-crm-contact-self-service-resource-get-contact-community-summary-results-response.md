# ComCrmContactSelfServiceResourceGetContactCommunitySummaryResultsResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetContactCommunitySummaryResultsResponse } from "crm/models/operations";

let value:
  ComCrmContactSelfServiceResourceGetContactCommunitySummaryResultsResponse = {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
      hasMore: true,
    },
    content: [
      {
        id: "323a12a6-90e4-fa30-caa4-63e9552ffb10",
        contact: {
          id: "19e631ac-4123-1099-d207-2a70fb126186",
          firstName: "John",
          lastName: "Smith",
          phone: {
            countryCode: "CYP",
            number: "744444121",
          },
          email: "johndoe@crm.com",
        },
        isOwner: true,
        relationshipId: "801b54cc-00c9-407d-86b7-77a9e8aefcf8",
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                                   | Type                                                                                                                                                                                                    | Required                                                                                                                                                                                                | Description                                                                                                                                                                                             |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                                | [operations.ComCrmContactSelfServiceResourceGetContactCommunitySummaryResultsPaging](../../models/operations/com-crm-contact-self-service-resource-get-contact-community-summary-results-paging.md)     | :heavy_minus_sign:                                                                                                                                                                                      | N/A                                                                                                                                                                                                     |
| `content`                                                                                                                                                                                               | [operations.ComCrmContactSelfServiceResourceGetContactCommunitySummaryResultsContent](../../models/operations/com-crm-contact-self-service-resource-get-contact-community-summary-results-content.md)[] | :heavy_minus_sign:                                                                                                                                                                                      | N/A                                                                                                                                                                                                     |