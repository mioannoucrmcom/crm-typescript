# AddContactIdentitySSPhone

The contact’s phone (required for phone/password or phone/OTP verification). Password is applicable only when authentication is phone/otp.

## Example Usage

```typescript
import { AddContactIdentitySSPhone } from "crm/models/operations";

let value: AddContactIdentitySSPhone = {
  number: "99123456",
  countryCode: "CYP",
};
```

## Fields

| Field                                                                                                         | Type                                                                                                          | Required                                                                                                      | Description                                                                                                   | Example                                                                                                       |
| ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `number`                                                                                                      | *string*                                                                                                      | :heavy_check_mark:                                                                                            | The phone number                                                                                              | 99123456                                                                                                      |
| `countryCode`                                                                                                 | [operations.AddContactIdentitySSCountryCode](../../models/operations/add-contact-identity-ss-country-code.md) | :heavy_check_mark:                                                                                            | The phone country code                                                                                        | CYP                                                                                                           |