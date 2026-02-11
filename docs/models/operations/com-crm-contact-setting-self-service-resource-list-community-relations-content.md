# ComCrmContactSettingSelfServiceResourceListCommunityRelationsContent

## Example Usage

```typescript
import { ComCrmContactSettingSelfServiceResourceListCommunityRelationsContent } from "crm/models/operations";

let value:
  ComCrmContactSettingSelfServiceResourceListCommunityRelationsContent = {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "Employees",
    isDefault: true,
  };
```

## Fields

| Field                                                                                                       | Type                                                                                                        | Required                                                                                                    | Description                                                                                                 | Example                                                                                                     |
| ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                        | *string*                                                                                                    | :heavy_minus_sign:                                                                                          | The entity identifier                                                                                       | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                        |
| `name`                                                                                                      | *string*                                                                                                    | :heavy_minus_sign:                                                                                          | The contact community relation name                                                                         | Employees                                                                                                   |
| `isDefault`                                                                                                 | *boolean*                                                                                                   | :heavy_minus_sign:                                                                                          | Determines whether this is the default community relation. A single Relation can be set as the default one. | true                                                                                                        |