# ComCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowanceRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowanceRequest } from "crmcom/models/operations";

let value:
  ComCrmContactSelfServiceResourceRemoveContactRelationshipProductAllowanceRequest =
    {
      id: "3afad71d-e015-4e98-a464-f438c93edcde",
      productAllowanceId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
      relationshipId: "891d84dd-4b3b-84b3-ba87-aa63fed3b88a",
    };
```

## Fields

| Field                                                    | Type                                                     | Required                                                 | Description                                              | Example                                                  |
| -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- |
| `id`                                                     | *string*                                                 | :heavy_check_mark:                                       | The contact (identifier) whose community will be updated | 3afad71d-e015-4e98-a464-f438c93edcde                     |
| `productAllowanceId`                                     | *string*                                                 | :heavy_check_mark:                                       | The product allowance(identifier) that will be deleted   | 891d84dd-4b3b-84b3-ba87-aa63fed3b88a                     |
| `relationshipId`                                         | *string*                                                 | :heavy_check_mark:                                       | The community person (identifier) that will be updated   | 891d84dd-4b3b-84b3-ba87-aa63fed3b88a                     |