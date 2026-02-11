# ComCrmContactSettingSelfServiceResourceListCommunityRelationsResponse

OK

## Example Usage

```typescript
import { ComCrmContactSettingSelfServiceResourceListCommunityRelationsResponse } from "crm/models/operations";

let value:
  ComCrmContactSettingSelfServiceResourceListCommunityRelationsResponse = {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
      hasMore: true,
    },
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "Employees",
        isDefault: true,
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                          | Type                                                                                                                                                                                           | Required                                                                                                                                                                                       | Description                                                                                                                                                                                    |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                       | [operations.ComCrmContactSettingSelfServiceResourceListCommunityRelationsPaging](../../models/operations/com-crm-contact-setting-self-service-resource-list-community-relations-paging.md)     | :heavy_minus_sign:                                                                                                                                                                             | N/A                                                                                                                                                                                            |
| `content`                                                                                                                                                                                      | [operations.ComCrmContactSettingSelfServiceResourceListCommunityRelationsContent](../../models/operations/com-crm-contact-setting-self-service-resource-list-community-relations-content.md)[] | :heavy_minus_sign:                                                                                                                                                                             | N/A                                                                                                                                                                                            |