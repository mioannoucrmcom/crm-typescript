# UpdateContactSSPhone

The contact’s phone

## Example Usage

```typescript
import { UpdateContactSSPhone } from "crm/models/operations";

let value: UpdateContactSSPhone = {
  type: "MOBILE",
  countryCode: "CYP",
  number: "99123456",
};
```

## Fields

| Field                                                                                              | Type                                                                                               | Required                                                                                           | Description                                                                                        | Example                                                                                            |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `type`                                                                                             | [operations.UpdateContactSSType](../../models/operations/update-contact-ss-type.md)                | :heavy_check_mark:                                                                                 | The phone type                                                                                     | MOBILE                                                                                             |
| `countryCode`                                                                                      | [operations.UpdateContactSSCountryCode](../../models/operations/update-contact-ss-country-code.md) | :heavy_minus_sign:                                                                                 | 3-character country code based on ISO 3166                                                         | CYP                                                                                                |
| `number`                                                                                           | *string*                                                                                           | :heavy_minus_sign:                                                                                 | The phone number                                                                                   | 99123456                                                                                           |