# ComCrmContactSelfServiceResourceAuthenticateRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceAuthenticateRequest } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceAuthenticateRequest = {
  body: {
    provider: "FACEBOOK",
    username: "johndoe@crm.com",
    password: "password1234",
    token: "234er43ergt34eett34",
    applicationId: "a9c09878-bf26-4969-8a35-61899d64302d",
    phone: {
      number: "99000000",
      countryCode: "CYP",
    },
    macAddress: "01-23-45-67-89-AB",
  },
};
```

## Fields

| Field                                                                                                                                                            | Type                                                                                                                                                             | Required                                                                                                                                                         | Description                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `apiKey`                                                                                                                                                         | *string*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | N/A                                                                                                                                                              |
| `body`                                                                                                                                                           | [operations.ComCrmContactSelfServiceResourceAuthenticateRequestBody](../../models/operations/com-crm-contact-self-service-resource-authenticate-request-body.md) | :heavy_check_mark:                                                                                                                                               | N/A                                                                                                                                                              |