# ComCrmContactSelfServiceResourceRequestOTPRequestBody

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceRequestOTPRequestBody } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceRequestOTPRequestBody = {
  method: "EMAIL",
  credentials: [
    {
      name: "BIRTHDATE",
      value: "1234567",
      giftPass: {
        email: "jonf.doe@gmail.com",
        phone: {
          number: "99000000",
          countryCode: "CYP",
        },
        pin: "132435",
        lastSpendAmount: 2.5,
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                              | Type                                                                                                                                               | Required                                                                                                                                           | Description                                                                                                                                        | Example                                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| `method`                                                                                                                                           | [operations.ComCrmContactSelfServiceResourceRequestOTPMethod](../../models/operations/com-crm-contact-self-service-resource-request-otp-method.md) | :heavy_check_mark:                                                                                                                                 | How to send the validation code                                                                                                                    | EMAIL                                                                                                                                              |
| `credentials`                                                                                                                                      | [operations.Credential](../../models/operations/credential.md)[]                                                                                   | :heavy_check_mark:                                                                                                                                 | Defines how a contact will be identified                                                                                                           |                                                                                                                                                    |