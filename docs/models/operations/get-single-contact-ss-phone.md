# GetSingleContactSSPhone

Contact phone information

## Example Usage

```typescript
import { GetSingleContactSSPhone } from "crmcom/models/operations";

let value: GetSingleContactSSPhone = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  type: "MOBILE",
  countryCode: "CYP",
  number: "99123456",
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               | Example                                                                                                   |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                      | *string*                                                                                                  | :heavy_minus_sign:                                                                                        | The entity identifier                                                                                     | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                      |
| `type`                                                                                                    | [operations.GetSingleContactSSPhoneType](../../models/operations/get-single-contact-ss-phone-type.md)     | :heavy_minus_sign:                                                                                        | The phone type                                                                                            | MOBILE                                                                                                    |
| `countryCode`                                                                                             | [operations.GetSingleContactSSCountryCode](../../models/operations/get-single-contact-ss-country-code.md) | :heavy_minus_sign:                                                                                        | 3-character country code based on ISO 3166                                                                | CYP                                                                                                       |
| `number`                                                                                                  | *string*                                                                                                  | :heavy_minus_sign:                                                                                        | The phone number                                                                                          | 99123456                                                                                                  |