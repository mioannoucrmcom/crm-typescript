# ComCrmServiceRequestSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmServiceRequestSelfServiceResourceListResponse } from "crm/models/operations";

let value: ComCrmServiceRequestSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      number: "SR1003",
      description: "Pot hole issues in Nicosia Main Road",
      comments: "Contact has been spoken to.",
      isResolved: true,
      stage: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "Response submitted",
        colour: "#FA89CB",
        order: 5,
      },
      address: {
        addressType: "HOME",
        addressName: "My house",
      },
      customFields: [
        {
          key: "back_office",
          value: "0001-12345",
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                                    | Type                                                                                                                                                     | Required                                                                                                                                                 | Description                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                 | [operations.ComCrmServiceRequestSelfServiceResourceListPaging](../../models/operations/com-crm-service-request-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                                       | N/A                                                                                                                                                      |
| `content`                                                                                                                                                | [operations.ComCrmServiceRequestSelfServiceResourceListContent](../../models/operations/com-crm-service-request-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                                       | N/A                                                                                                                                                      |