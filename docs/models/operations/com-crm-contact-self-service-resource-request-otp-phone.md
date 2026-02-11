# ComCrmContactSelfServiceResourceRequestOTPPhone

The contact’s phone

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceRequestOTPPhone } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceRequestOTPPhone = {
  number: "99000000",
  countryCode: "CYP",
};
```

## Fields

| Field                                                                                                                                                         | Type                                                                                                                                                          | Required                                                                                                                                                      | Description                                                                                                                                                   | Example                                                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `number`                                                                                                                                                      | *string*                                                                                                                                                      | :heavy_check_mark:                                                                                                                                            | The contact’s phone number                                                                                                                                    | 99000000                                                                                                                                                      |
| `countryCode`                                                                                                                                                 | [operations.ComCrmContactSelfServiceResourceRequestOTPCountryCode](../../models/operations/com-crm-contact-self-service-resource-request-otp-country-code.md) | :heavy_check_mark:                                                                                                                                            | The contact’s phone country code                                                                                                                              | CYP                                                                                                                                                           |