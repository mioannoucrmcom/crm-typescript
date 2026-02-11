# GetSingleContactSSPassport

Contact’s passport information

## Example Usage

```typescript
import { GetSingleContactSSPassport } from "crmcom/models/operations";

let value: GetSingleContactSSPassport = {
  number: "AK123456",
  issuingCountryCode: "CYP",
  expirationDate: 1677673128,
};
```

## Fields

| Field                                                                                                                                     | Type                                                                                                                                      | Required                                                                                                                                  | Description                                                                                                                               | Example                                                                                                                                   |
| ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| `number`                                                                                                                                  | *string*                                                                                                                                  | :heavy_minus_sign:                                                                                                                        | Passport number                                                                                                                           | AK123456                                                                                                                                  |
| `issuingCountryCode`                                                                                                                      | [operations.GetSingleContactSSPassportIssuingCountryCode](../../models/operations/get-single-contact-ss-passport-issuing-country-code.md) | :heavy_minus_sign:                                                                                                                        | 3-character country code based on ISO 3166                                                                                                | CYP                                                                                                                                       |
| `expirationDate`                                                                                                                          | *number*                                                                                                                                  | :heavy_minus_sign:                                                                                                                        | Passport’s expiry date                                                                                                                    | 1677673128                                                                                                                                |