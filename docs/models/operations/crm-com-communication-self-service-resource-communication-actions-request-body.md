# CrmComCommunicationSelfServiceResourceCommunicationActionsRequestBody

## Example Usage

```typescript
import { CrmComCommunicationSelfServiceResourceCommunicationActionsRequestBody } from "crmcom/models/operations";

let value:
  CrmComCommunicationSelfServiceResourceCommunicationActionsRequestBody = {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    viewed: true,
    archived: true,
  };
```

## Fields

| Field                                      | Type                                       | Required                                   | Description                                | Example                                    |
| ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ | ------------------------------------------ |
| `id`                                       | *string*                                   | :heavy_minus_sign:                         | The entity identifier that will be created | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0       |
| `viewed`                                   | *boolean*                                  | :heavy_check_mark:                         | Sets the communication as viewed           | true                                       |
| `archived`                                 | *boolean*                                  | :heavy_check_mark:                         | Sets the communication as archived         | true                                       |