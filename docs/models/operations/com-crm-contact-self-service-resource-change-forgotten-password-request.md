# ComCrmContactSelfServiceResourceChangeForgottenPasswordRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceChangeForgottenPasswordRequest } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceChangeForgottenPasswordRequest = {
  token: "j677enty-23sfsfsf23456798vgp",
  password: "wsxcde421qadfg",
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       | Example                                                                           |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `token`                                                                           | *string*                                                                          | :heavy_check_mark:                                                                | The token that will verify that the client (that performs such action) is trusted | j677enty-23sfsfsf23456798vgp                                                      |
| `password`                                                                        | *string*                                                                          | :heavy_check_mark:                                                                | The new password                                                                  | wsxcde421qadfg                                                                    |