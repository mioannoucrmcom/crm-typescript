# ComCrmContactSelfServiceResourceRemoveFileRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceRemoveFileRequest } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceRemoveFileRequest = {
  attachmentId: "<id>",
  id: "<id>",
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `attachmentId`                                                | *string*                                                      | :heavy_check_mark:                                            | The attachment (identifier) to be deleted                     |
| `id`                                                          | *string*                                                      | :heavy_check_mark:                                            | The contact (identifier) for which attachment will be deleted |