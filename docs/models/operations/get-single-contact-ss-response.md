# GetSingleContactSSResponse

OK

## Example Usage

```typescript
import { GetSingleContactSSResponse } from "crmcom/models/operations";

let value: GetSingleContactSSResponse = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  code: "100000001908",
  firstName: "John",
  middleName: "Alias",
  lastName: "Doe",
  companyName: "Smith & Sons Ltd.",
  companyProfile: {
    registrationNumber: "EPM869233102",
    registrationCountry: "CYP",
    taxReferenceNumber: "TPS90398813",
    vatRegistrationNumber: "1206523T",
    industry: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Universal Name",
    },
    subIndustries: [
      {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
      },
    ],
  },
  languageCode: "EN",
  email: "john.smith@crm.com",
  phone: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    type: "MOBILE",
    countryCode: "CYP",
    number: "99123456",
  },
  demographics: {
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
  },
  referralCode: "REF123",
  smsOptOut: false,
  emailOptOut: false,
  countryOfAgreement: "CYP",
  loyaltyIdentifiers: [
    {
      identifier: "100000001908",
    },
  ],
  customFields: [
    {
      key: "back_office",
      value: "0001-12345",
    },
  ],
  wallet: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    code: "2131424123",
  },
  creatives: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      width: 2159,
      height: 3075,
      format: "jpg",
      url: "https://assets.crm.com/image/offer.jpg",
      publicId: "crm-com/image",
      media: [
        {
          width: 200,
          height: 300,
          url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                         | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   | Example                                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                          | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The entity identifier                                                                                                                                                                         | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                          |
| `code`                                                                                                                                                                                        | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The contact code                                                                                                                                                                              | 100000001908                                                                                                                                                                                  |
| `type`                                                                                                                                                                                        | [operations.GetSingleContactSSType](../../models/operations/get-single-contact-ss-type.md)                                                                                                    | :heavy_minus_sign:                                                                                                                                                                            | Contact type - can be PERSON or COMPANY                                                                                                                                                       |                                                                                                                                                                                               |
| `firstName`                                                                                                                                                                                   | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The contact’s first name                                                                                                                                                                      | John                                                                                                                                                                                          |
| `middleName`                                                                                                                                                                                  | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The contact’s middle name                                                                                                                                                                     | Alias                                                                                                                                                                                         |
| `lastName`                                                                                                                                                                                    | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The contact’s last name                                                                                                                                                                       | Doe                                                                                                                                                                                           |
| `companyName`                                                                                                                                                                                 | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The company name if the contact type is 'COMPANY'                                                                                                                                             | Smith & Sons Ltd.                                                                                                                                                                             |
| `companyProfile`                                                                                                                                                                              | [operations.GetSingleContactSSCompanyProfile](../../models/operations/get-single-contact-ss-company-profile.md)                                                                               | :heavy_minus_sign:                                                                                                                                                                            | Information about the company's profile, applicable only for contacts of type 'COMPANY'                                                                                                       |                                                                                                                                                                                               |
| `languageCode`                                                                                                                                                                                | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The contact’s selected language for communications and translations                                                                                                                           | EN                                                                                                                                                                                            |
| `email`                                                                                                                                                                                       | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The contact’s email address                                                                                                                                                                   | john.smith@crm.com                                                                                                                                                                            |
| `phone`                                                                                                                                                                                       | [operations.GetSingleContactSSPhone](../../models/operations/get-single-contact-ss-phone.md)                                                                                                  | :heavy_minus_sign:                                                                                                                                                                            | Contact phone information                                                                                                                                                                     |                                                                                                                                                                                               |
| `demographics`                                                                                                                                                                                | [operations.GetSingleContactSSDemographics](../../models/operations/get-single-contact-ss-demographics.md)                                                                                    | :heavy_minus_sign:                                                                                                                                                                            | N/A                                                                                                                                                                                           |                                                                                                                                                                                               |
| `referralCode`                                                                                                                                                                                | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The contact referral code used when referring friends                                                                                                                                         | REF123                                                                                                                                                                                        |
| `smsOptOut`                                                                                                                                                                                   | *boolean*                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                            | Has the contact opted-out from receiving text messages (sms)?                                                                                                                                 | false                                                                                                                                                                                         |
| `emailOptOut`                                                                                                                                                                                 | *boolean*                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                            | Has the contact opted-out from receiving emails?                                                                                                                                              | false                                                                                                                                                                                         |
| `countryOfAgreement`                                                                                                                                                                          | [operations.GetSingleContactSSCountryOfAgreement](../../models/operations/get-single-contact-ss-country-of-agreement.md)                                                                      | :heavy_minus_sign:                                                                                                                                                                            | 3-char country code of the contact based on locale, this will be used to determine pricing and taxes                                                                                          | CYP                                                                                                                                                                                           |
| `avatarUrl`                                                                                                                                                                                   | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | Avatar URL                                                                                                                                                                                    |                                                                                                                                                                                               |
| `loyaltyIdentifiers`                                                                                                                                                                          | [operations.LoyaltyIdentifier](../../models/operations/loyalty-identifier.md)[]                                                                                                               | :heavy_minus_sign:                                                                                                                                                                            | The loyalty identifiers used to identify the contact (e.g. a loyalty card number from an external system)                                                                                     |                                                                                                                                                                                               |
| `customFields`                                                                                                                                                                                | [operations.GetSingleContactSSCustomField](../../models/operations/get-single-contact-ss-custom-field.md)[]                                                                                   | :heavy_minus_sign:                                                                                                                                                                            | The custom fields of contact                                                                                                                                                                  |                                                                                                                                                                                               |
| `wallet`                                                                                                                                                                                      | [operations.GetSingleContactSSWallet](../../models/operations/get-single-contact-ss-wallet.md)                                                                                                | :heavy_minus_sign:                                                                                                                                                                            | Contact wallet information                                                                                                                                                                    |                                                                                                                                                                                               |
| `creatives`                                                                                                                                                                                   | [operations.GetSingleContactSSCreative](../../models/operations/get-single-contact-ss-creative.md)[]                                                                                          | :heavy_minus_sign:                                                                                                                                                                            | A creative is an object that contains all the data required for visually rendering an image responsively. The object contains the initial image and a number of scale versions of it (srcset) |                                                                                                                                                                                               |
| `viewedOnboardingCards`                                                                                                                                                                       | *boolean*                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                            | Contact viewed the onboarding cards                                                                                                                                                           |                                                                                                                                                                                               |