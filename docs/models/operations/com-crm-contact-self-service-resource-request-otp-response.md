# ComCrmContactSelfServiceResourceRequestOTPResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceRequestOTPResponse } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceRequestOTPResponse = {
  obfuscatedValue: "+35799***834",
  authOtp: "731e4023-4c04-4278-8eb5-240651317e46",
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   | Example                                                       |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `obfuscatedValue`                                             | *string*                                                      | :heavy_minus_sign:                                            | The obfuscated value of the email or sms used to send the otp | +35799***834                                                  |
| `authOtp`                                                     | *string*                                                      | :heavy_minus_sign:                                            | The one time password authentication identifier               | 731e4023-4c04-4278-8eb5-240651317e46                          |