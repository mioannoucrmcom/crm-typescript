# ComCrmAccountSelfServiceResourceUpdateAccountRequest

## Example Usage

```typescript
import { ComCrmAccountSelfServiceResourceUpdateAccountRequest } from "crm/models/operations";

let value: ComCrmAccountSelfServiceResourceUpdateAccountRequest = {
  id: "AF1D8C778F6540E29EECEABCD8711C3A",
  body: {
    classificationId: "8F95E1B6FEC1487E88A9AAF3C214A870",
    isPrimary: true,
    billingAddressId: "974A084BA7794F6D9A2F94A521DDCDAB",
  },
};
```

## Fields

| Field                                                                                                                                                               | Type                                                                                                                                                                | Required                                                                                                                                                            | Description                                                                                                                                                         | Example                                                                                                                                                             |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                | *string*                                                                                                                                                            | :heavy_check_mark:                                                                                                                                                  | The account identifier that will be updated                                                                                                                         | AF1D8C778F6540E29EECEABCD8711C3A                                                                                                                                    |
| `body`                                                                                                                                                              | [operations.ComCrmAccountSelfServiceResourceUpdateAccountRequestBody](../../models/operations/com-crm-account-self-service-resource-update-account-request-body.md) | :heavy_check_mark:                                                                                                                                                  | N/A                                                                                                                                                                 |                                                                                                                                                                     |