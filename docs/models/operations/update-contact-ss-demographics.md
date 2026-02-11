# UpdateContactSSDemographics

Information about the person demographics

## Example Usage

```typescript
import { UpdateContactSSDemographics } from "crmcom/models/operations";

let value: UpdateContactSSDemographics = {
  gender: "FEMALE",
  dateOfBirth: {
    year: 1948,
    month: 3,
    day: 1,
  },
  nameDay: {
    month: 6,
    day: 8,
  },
  passport: {
    number: "AK123456",
    issuingCountryCode: "CYP",
    expirationDate: 1677673128,
  },
  idDetails: null,
  statutoryNumber: "231224-8424406",
};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         | Example                                                                                             |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `gender`                                                                                            | [operations.UpdateContactSSGender](../../models/operations/update-contact-ss-gender.md)             | :heavy_minus_sign:                                                                                  | Contact’s gender information                                                                        | FEMALE                                                                                              |
| `dateOfBirth`                                                                                       | [operations.UpdateContactSSDateOfBirth](../../models/operations/update-contact-ss-date-of-birth.md) | :heavy_minus_sign:                                                                                  | Contact’s date of birth                                                                             |                                                                                                     |
| `nameDay`                                                                                           | [operations.UpdateContactSSNameDay](../../models/operations/update-contact-ss-name-day.md)          | :heavy_minus_sign:                                                                                  | Contact’s nameday information                                                                       |                                                                                                     |
| `passport`                                                                                          | [operations.UpdateContactSSPassport](../../models/operations/update-contact-ss-passport.md)         | :heavy_minus_sign:                                                                                  | Contact’s passport information                                                                      |                                                                                                     |
| `idDetails`                                                                                         | [operations.UpdateContactSSIdDetails](../../models/operations/update-contact-ss-id-details.md)      | :heavy_minus_sign:                                                                                  | Contact’s ID information                                                                            |                                                                                                     |
| `statutoryNumber`                                                                                   | *string*                                                                                            | :heavy_minus_sign:                                                                                  | The contact’s unique statutory number                                                               | 231224-8424406                                                                                      |