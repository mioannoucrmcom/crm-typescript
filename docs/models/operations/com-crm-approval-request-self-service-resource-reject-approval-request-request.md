# ComCrmApprovalRequestSelfServiceResourceRejectApprovalRequestRequest

## Example Usage

```typescript
import { ComCrmApprovalRequestSelfServiceResourceRejectApprovalRequestRequest } from "crm/models/operations";

let value:
  ComCrmApprovalRequestSelfServiceResourceRejectApprovalRequestRequest = {
    token: "2fa42de0-38a0-1e86-b813-d370c35b082c",
  };
```

## Fields

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               | Example                                                                                   |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `token`                                                                                   | *string*                                                                                  | :heavy_check_mark:                                                                        | The token that will verify that the client is trusted and will reject the related request | 2fa42de0-38a0-1e86-b813-d370c35b082c                                                      |