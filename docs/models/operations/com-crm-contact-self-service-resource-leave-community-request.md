# ComCrmContactSelfServiceResourceLeaveCommunityRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceLeaveCommunityRequest } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceLeaveCommunityRequest = {
  communityOwnerId: "ccc945d8-1bda-a11c-d378-23c29947c2a3",
  id: "5096c4d4-c387-9888-d631-80e74546e2db",
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    | Example                                                                                        |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `communityOwnerId`                                                                             | *string*                                                                                       | :heavy_check_mark:                                                                             | The community owner contact (identifier) that his/her member will leave from his/her community | ccc945d8-1bda-a11c-d378-23c29947c2a3                                                           |
| `id`                                                                                           | *string*                                                                                       | :heavy_check_mark:                                                                             | The contact (identifier) that will leave as a member from a community                          | 5096c4d4-c387-9888-d631-80e74546e2db                                                           |