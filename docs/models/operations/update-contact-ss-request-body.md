# UpdateContactSSRequestBody

## Example Usage

```typescript
import { UpdateContactSSRequestBody } from "crm/models/operations";

let value: UpdateContactSSRequestBody = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  firstName: "John",
  middleName: "Patrick",
  lastName: "Smith",
  languageCode: "EN",
  email: "john.smith@gmail.com",
  phone: {
    type: "MOBILE",
    countryCode: "CYP",
    number: "99123456",
  },
  demographics: {
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
    idDetails: {
      number: "809251833",
      issuingCountryCode: "CYP",
      expirationDate: 1709295528,
    },
    statutoryNumber: "231224-8424406",
  },
  smsOptOut: false,
  emailOptOut: false,
  customFields: [
    {
      key: "back_office",
      value: "0001-12345",
    },
  ],
  companyProfile: {
    registrationNumber: "EPM869233102",
    registrationCountry: "CYP",
    taxReferenceNumber: "TPS90398813",
    vatRegistrationNumber: "1206523T",
    industryId: "69350edc-e0dc-4e2d-a8a1-8f26a2eacc09",
    subIndustries: null,
  },
};
```

## Fields

| Field                                                                                                    | Type                                                                                                     | Required                                                                                                 | Description                                                                                              | Example                                                                                                  |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                     | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | The entity identifier that will be created                                                               | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                     |
| `firstName`                                                                                              | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | Contact’s first name                                                                                     | John                                                                                                     |
| `middleName`                                                                                             | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | Contact’s middle name                                                                                    | Patrick                                                                                                  |
| `lastName`                                                                                               | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | Contact’s last name                                                                                      | Smith                                                                                                    |
| `languageCode`                                                                                           | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | The contact’s selected language, used for communications, translations etc.                              | EN                                                                                                       |
| `email`                                                                                                  | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | The contact’s email address                                                                              | john.smith@gmail.com                                                                                     |
| `phone`                                                                                                  | [operations.UpdateContactSSPhone](../../models/operations/update-contact-ss-phone.md)                    | :heavy_minus_sign:                                                                                       | The contact’s phone                                                                                      |                                                                                                          |
| `demographics`                                                                                           | [operations.UpdateContactSSDemographics](../../models/operations/update-contact-ss-demographics.md)      | :heavy_minus_sign:                                                                                       | Information about the person demographics                                                                |                                                                                                          |
| `smsOptOut`                                                                                              | *boolean*                                                                                                | :heavy_minus_sign:                                                                                       | Has the contact opted out from receiving text messages (sms)?                                            | false                                                                                                    |
| `emailOptOut`                                                                                            | *boolean*                                                                                                | :heavy_minus_sign:                                                                                       | Has the contact opted out from receiving emails?                                                         | false                                                                                                    |
| `customFields`                                                                                           | [operations.UpdateContactSSCustomField](../../models/operations/update-contact-ss-custom-field.md)[]     | :heavy_minus_sign:                                                                                       | The custom fields of contact                                                                             |                                                                                                          |
| `companyName`                                                                                            | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | A company’s name (applicable only if contact type is COMPANY)                                            |                                                                                                          |
| `companyProfile`                                                                                         | [operations.UpdateContactSSCompanyProfile](../../models/operations/update-contact-ss-company-profile.md) | :heavy_minus_sign:                                                                                       | A company’s profile (applicable only if contact type is COMPANY)                                         |                                                                                                          |