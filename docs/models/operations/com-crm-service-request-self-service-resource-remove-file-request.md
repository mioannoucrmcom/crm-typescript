# ComCrmServiceRequestSelfServiceResourceRemoveFileRequest

## Example Usage

```typescript
import { ComCrmServiceRequestSelfServiceResourceRemoveFileRequest } from "crm/models/operations";

let value: ComCrmServiceRequestSelfServiceResourceRemoveFileRequest = {
  attachmentId: "8dfc2223-edca-f05d-820b-dc96ba9df2c2",
  id: "6b888b83-b418-752f-604d-0653cf65885d",
};
```

## Fields

| Field                                                                 | Type                                                                  | Required                                                              | Description                                                           | Example                                                               |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `attachmentId`                                                        | *string*                                                              | :heavy_check_mark:                                                    | The attachment (identifier) to be deleted                             | 8dfc2223-edca-f05d-820b-dc96ba9df2c2                                  |
| `id`                                                                  | *string*                                                              | :heavy_check_mark:                                                    | The service request (identifier) for which attachment will be deleted | 6b888b83-b418-752f-604d-0653cf65885d                                  |