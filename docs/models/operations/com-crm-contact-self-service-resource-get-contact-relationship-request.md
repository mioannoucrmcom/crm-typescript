# ComCrmContactSelfServiceResourceGetContactRelationshipRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetContactRelationshipRequest } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceGetContactRelationshipRequest = {
  id: "3afad71d-e015-4e98-a464-f438c93edcde",
  relationshipId: "dc01f65b-a482-48f1-9fda-c163df72f28f",
};
```

## Fields

| Field                                                                                                       | Type                                                                                                        | Required                                                                                                    | Description                                                                                                 | Example                                                                                                     |
| ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                        | *string*                                                                                                    | :heavy_check_mark:                                                                                          | The contact (identifier) whose community will be retrieved                                                  | 3afad71d-e015-4e98-a464-f438c93edcde                                                                        |
| `relationshipId`                                                                                            | *string*                                                                                                    | :heavy_check_mark:                                                                                          | The community person (identifier) that will be retrieved                                                    | dc01f65b-a482-48f1-9fda-c163df72f28f                                                                        |
| `includeRemainingAllowance`                                                                                 | *boolean*                                                                                                   | :heavy_minus_sign:                                                                                          | Defaults to false. If set to true, the member’s remaining accumulated amounts are included in the response. |                                                                                                             |