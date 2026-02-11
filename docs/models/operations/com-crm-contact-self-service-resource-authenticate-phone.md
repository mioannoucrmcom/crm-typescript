# ComCrmContactSelfServiceResourceAuthenticatePhone

The contact’s phone

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceAuthenticatePhone } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceAuthenticatePhone = {
  number: "99000000",
  countryCode: "CYP",
};
```

## Fields

| Field                                                                                                                                                            | Type                                                                                                                                                             | Required                                                                                                                                                         | Description                                                                                                                                                      | Example                                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `number`                                                                                                                                                         | *string*                                                                                                                                                         | :heavy_check_mark:                                                                                                                                               | The contact’s phone number                                                                                                                                       | 99000000                                                                                                                                                         |
| `countryCode`                                                                                                                                                    | [operations.ComCrmContactSelfServiceResourceAuthenticateCountryCode](../../models/operations/com-crm-contact-self-service-resource-authenticate-country-code.md) | :heavy_check_mark:                                                                                                                                               | The contact’s phone country code                                                                                                                                 | CYP                                                                                                                                                              |