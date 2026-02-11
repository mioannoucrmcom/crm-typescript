# ComCrmAccountSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmAccountSelfServiceResourceListResponse } from "crmcom/models/operations";

let value: ComCrmAccountSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      isPrimary: true,
      name: "ACR123456-JohnDoe",
      number: "ACR123456",
      state: "ACTIVE",
      currencyCode: "EUR",
    },
  ],
};
```

## Fields

| Field                                                                                                                                     | Type                                                                                                                                      | Required                                                                                                                                  | Description                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                  | [operations.ComCrmAccountSelfServiceResourceListPaging](../../models/operations/com-crm-account-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                        | N/A                                                                                                                                       |
| `content`                                                                                                                                 | [operations.ComCrmAccountSelfServiceResourceListContent](../../models/operations/com-crm-account-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                        | N/A                                                                                                                                       |