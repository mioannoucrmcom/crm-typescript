# GetSingleContactSSCompanyProfile

Information about the company's profile, applicable only for contacts of type 'COMPANY'

## Example Usage

```typescript
import { GetSingleContactSSCompanyProfile } from "crmcom/models/operations";

let value: GetSingleContactSSCompanyProfile = {
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
};
```

## Fields

| Field                                                                                                                     | Type                                                                                                                      | Required                                                                                                                  | Description                                                                                                               | Example                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| `registrationNumber`                                                                                                      | *string*                                                                                                                  | :heavy_minus_sign:                                                                                                        | Company’s registration number                                                                                             | EPM869233102                                                                                                              |
| `registrationCountry`                                                                                                     | [operations.GetSingleContactSSRegistrationCountry](../../models/operations/get-single-contact-ss-registration-country.md) | :heavy_minus_sign:                                                                                                        | 3-character country code based on ISO 3166                                                                                | CYP                                                                                                                       |
| `taxReferenceNumber`                                                                                                      | *string*                                                                                                                  | :heavy_minus_sign:                                                                                                        | The company’s tax reference number                                                                                        | TPS90398813                                                                                                               |
| `vatRegistrationNumber`                                                                                                   | *string*                                                                                                                  | :heavy_minus_sign:                                                                                                        | The company VAT registration numnber                                                                                      | 1206523T                                                                                                                  |
| `industry`                                                                                                                | [operations.Industry](../../models/operations/industry.md)                                                                | :heavy_minus_sign:                                                                                                        | The company’s Industry details                                                                                            |                                                                                                                           |
| `subIndustries`                                                                                                           | [operations.GetSingleContactSSSubIndustry](../../models/operations/get-single-contact-ss-sub-industry.md)[]               | :heavy_minus_sign:                                                                                                        | The company’s Sub-Industries details                                                                                      |                                                                                                                           |