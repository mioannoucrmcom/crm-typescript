# Authentication

Details on how customers can auth by the app

## Example Usage

```typescript
import { Authentication } from "crm/models/operations";

let value: Authentication = {
  emailPassword: true,
  emailOtp: false,
  smsOtp: true,
  facebook: {
    isSupported: true,
    appId: "sfsdf-23-we-wer-3ew-dw",
  },
  demoContact: {
    isSupported: true,
    contact: {
      id: "76ee374d-cd38-4cde-9fa3-4eaa26e67a06",
      name: "John Doe",
    },
    otp: "123456",
  },
  guestContact: {
    isSupported: true,
    contact: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "John Doe",
    },
  },
  sso: {
    isSupported: true,
  },
};
```

## Fields

| Field                                                                                                         | Type                                                                                                          | Required                                                                                                      | Description                                                                                                   | Example                                                                                                       |
| ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `emailPassword`                                                                                               | *boolean*                                                                                                     | :heavy_minus_sign:                                                                                            | Supported authentication based on email and password                                                          | true                                                                                                          |
| `emailOtp`                                                                                                    | *boolean*                                                                                                     | :heavy_minus_sign:                                                                                            | Supported authentication based on email and one time password                                                 | false                                                                                                         |
| `smsOtp`                                                                                                      | *boolean*                                                                                                     | :heavy_minus_sign:                                                                                            | Supported authentication based on one time password                                                           | true                                                                                                          |
| `facebook`                                                                                                    | [operations.Facebook](../../models/operations/facebook.md)                                                    | :heavy_minus_sign:                                                                                            | Defines whether contacts can register & sign-in based on Facebook (including Facebook authentication details) |                                                                                                               |
| `google`                                                                                                      | [operations.Google](../../models/operations/google.md)                                                        | :heavy_minus_sign:                                                                                            | N/A                                                                                                           |                                                                                                               |
| `demoContact`                                                                                                 | [operations.DemoContact](../../models/operations/demo-contact.md)                                             | :heavy_minus_sign:                                                                                            | The contact assigned as demo contact (used for app store verification purposes)                               |                                                                                                               |
| `guestContact`                                                                                                | [operations.GuestContact](../../models/operations/guest-contact.md)                                           | :heavy_minus_sign:                                                                                            | The contact assigned as guest contact (used for continuing as guest in app)                                   |                                                                                                               |
| `sso`                                                                                                         | [operations.Sso](../../models/operations/sso.md)                                                              | :heavy_minus_sign:                                                                                            | Support contacts authentication using an Open ID Connect provider (that enables single-sign-on)               |                                                                                                               |