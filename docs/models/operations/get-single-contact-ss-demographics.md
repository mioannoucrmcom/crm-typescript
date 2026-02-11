# GetSingleContactSSDemographics

## Example Usage

```typescript
import { GetSingleContactSSDemographics } from "crm/models/operations";

let value: GetSingleContactSSDemographics = {
  gender: "MALE",
  nameDay: {
    month: 10,
    day: 4,
  },
  dateOfBirth: {
    year: 2018,
    month: 10,
    day: 16,
  },
  passport: {
    number: "AK123456",
    issuingCountryCode: "CYP",
    expirationDate: 1677673128,
  },
  statutoryNumber: "231224-8424406",
  idDetails: {
    number: "809251833",
    issuingCountryCode: "CYP",
    expirationDate: 1677673128,
  },
};
```

## Fields

| Field                                                                                                      | Type                                                                                                       | Required                                                                                                   | Description                                                                                                | Example                                                                                                    |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| `gender`                                                                                                   | [operations.GetSingleContactSSGender](../../models/operations/get-single-contact-ss-gender.md)             | :heavy_minus_sign:                                                                                         | Contact’s gender information                                                                               | MALE                                                                                                       |
| `nameDay`                                                                                                  | [operations.GetSingleContactSSNameDay](../../models/operations/get-single-contact-ss-name-day.md)          | :heavy_minus_sign:                                                                                         | Contact’s date of birth                                                                                    |                                                                                                            |
| `dateOfBirth`                                                                                              | [operations.GetSingleContactSSDateOfBirth](../../models/operations/get-single-contact-ss-date-of-birth.md) | :heavy_minus_sign:                                                                                         | Contact’s nameday information                                                                              |                                                                                                            |
| `passport`                                                                                                 | [operations.GetSingleContactSSPassport](../../models/operations/get-single-contact-ss-passport.md)         | :heavy_minus_sign:                                                                                         | Contact’s passport information                                                                             |                                                                                                            |
| `statutoryNumber`                                                                                          | *string*                                                                                                   | :heavy_minus_sign:                                                                                         | The contact’s unique statutory number                                                                      | 231224-8424406                                                                                             |
| `idDetails`                                                                                                | [operations.GetSingleContactSSIdDetails](../../models/operations/get-single-contact-ss-id-details.md)      | :heavy_minus_sign:                                                                                         | Contact’s ID information                                                                                   |                                                                                                            |