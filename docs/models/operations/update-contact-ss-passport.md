# UpdateContactSSPassport

Contact’s passport information

## Example Usage

```typescript
import { UpdateContactSSPassport } from "crmcom/models/operations";

let value: UpdateContactSSPassport = {
  number: "AK123456",
  issuingCountryCode: "CYP",
  expirationDate: 1677673128,
};
```

## Fields

| Field                                                                                                                              | Type                                                                                                                               | Required                                                                                                                           | Description                                                                                                                        | Example                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| `number`                                                                                                                           | *string*                                                                                                                           | :heavy_check_mark:                                                                                                                 | Passport number                                                                                                                    | AK123456                                                                                                                           |
| `issuingCountryCode`                                                                                                               | [operations.UpdateContactSSPassportIssuingCountryCode](../../models/operations/update-contact-ss-passport-issuing-country-code.md) | :heavy_check_mark:                                                                                                                 | 3-character country code based on ISO 3166                                                                                         | CYP                                                                                                                                |
| `expirationDate`                                                                                                                   | *number*                                                                                                                           | :heavy_check_mark:                                                                                                                 | Passport’s expiry date                                                                                                             | 1677673128                                                                                                                         |