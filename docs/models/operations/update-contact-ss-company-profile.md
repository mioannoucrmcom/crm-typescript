# UpdateContactSSCompanyProfile

A company’s profile (applicable only if contact type is COMPANY)

## Example Usage

```typescript
import { UpdateContactSSCompanyProfile } from "crm/models/operations";

let value: UpdateContactSSCompanyProfile = {
  registrationNumber: "EPM869233102",
  registrationCountry: "CYP",
  taxReferenceNumber: "TPS90398813",
  vatRegistrationNumber: "1206523T",
  industryId: "69350edc-e0dc-4e2d-a8a1-8f26a2eacc09",
  subIndustries: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    },
  ],
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        | Example                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `registrationNumber`                                                                                               | *string*                                                                                                           | :heavy_minus_sign:                                                                                                 | Company’s registration number                                                                                      | EPM869233102                                                                                                       |
| `registrationCountry`                                                                                              | [operations.UpdateContactSSRegistrationCountry](../../models/operations/update-contact-ss-registration-country.md) | :heavy_minus_sign:                                                                                                 | 3-character country code based on ISO 3166                                                                         | CYP                                                                                                                |
| `taxReferenceNumber`                                                                                               | *string*                                                                                                           | :heavy_minus_sign:                                                                                                 | The company’s tax reference number                                                                                 | TPS90398813                                                                                                        |
| `vatRegistrationNumber`                                                                                            | *string*                                                                                                           | :heavy_minus_sign:                                                                                                 | The company VAT registration number                                                                                | 1206523T                                                                                                           |
| `industryId`                                                                                                       | *string*                                                                                                           | :heavy_minus_sign:                                                                                                 | Id for company’s industry                                                                                          | 69350edc-e0dc-4e2d-a8a1-8f26a2eacc09                                                                               |
| `subIndustries`                                                                                                    | [operations.UpdateContactSSSubIndustry](../../models/operations/update-contact-ss-sub-industry.md)[]               | :heavy_minus_sign:                                                                                                 | Ids for company’s sub-industries                                                                                   |                                                                                                                    |