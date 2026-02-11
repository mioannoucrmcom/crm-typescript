# ComCrmContactSelfServiceResourceValidateOTPRequestBody

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceValidateOTPRequestBody } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceValidateOTPRequestBody = {
  code: "123456",
  authOtp: "47c7-318202dbe45d",
};
```

## Fields

| Field                                                                                                                         | Type                                                                                                                          | Required                                                                                                                      | Description                                                                                                                   | Example                                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| `code`                                                                                                                        | *string*                                                                                                                      | :heavy_check_mark:                                                                                                            | The one time password that was sent to the contact and should be used for verification purposes                               | 123456                                                                                                                        |
| `authOtp`                                                                                                                     | *string*                                                                                                                      | :heavy_check_mark:                                                                                                            | The one time password authentication identifier that is generated as per otp request and will be used for validating such otp | 47c7-318202dbe45d                                                                                                             |