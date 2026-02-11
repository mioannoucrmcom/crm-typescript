# ComCrmContactSelfServiceResourceGetContactPersonRemainingAllowanceResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetContactPersonRemainingAllowanceResponse } from "crm/models/operations";

let value:
  ComCrmContactSelfServiceResourceGetContactPersonRemainingAllowanceResponse = {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
      hasMore: true,
    },
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        currency: "EUR",
        itemType: "PRODUCT",
        itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
        name: "Bronze",
        measurementUnit: {
          name: "Gigabytes",
          displayName: "GB",
        },
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                                     | Type                                                                                                                                                                                                      | Required                                                                                                                                                                                                  | Description                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                                  | [operations.ComCrmContactSelfServiceResourceGetContactPersonRemainingAllowancePaging](../../models/operations/com-crm-contact-self-service-resource-get-contact-person-remaining-allowance-paging.md)     | :heavy_minus_sign:                                                                                                                                                                                        | N/A                                                                                                                                                                                                       |
| `content`                                                                                                                                                                                                 | [operations.ComCrmContactSelfServiceResourceGetContactPersonRemainingAllowanceContent](../../models/operations/com-crm-contact-self-service-resource-get-contact-person-remaining-allowance-content.md)[] | :heavy_minus_sign:                                                                                                                                                                                        | N/A                                                                                                                                                                                                       |