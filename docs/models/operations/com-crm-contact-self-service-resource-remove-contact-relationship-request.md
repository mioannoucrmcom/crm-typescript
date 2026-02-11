# ComCrmContactSelfServiceResourceRemoveContactRelationshipRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceRemoveContactRelationshipRequest } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceRemoveContactRelationshipRequest = {
  id: "3afad71d-e015-4e98-a464-f438c93edcde",
  relationshipId: "bfd3cc67-2a4b-2900-6fcc-2ad3341f5495",
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              | Example                                                                                  |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `id`                                                                                     | *string*                                                                                 | :heavy_check_mark:                                                                       | The contact (identifier) whose community will be updated, by removing an existing member | 3afad71d-e015-4e98-a464-f438c93edcde                                                     |
| `relationshipId`                                                                         | *string*                                                                                 | :heavy_check_mark:                                                                       | The community person (identifier) that will be deleted                                   | bfd3cc67-2a4b-2900-6fcc-2ad3341f5495                                                     |