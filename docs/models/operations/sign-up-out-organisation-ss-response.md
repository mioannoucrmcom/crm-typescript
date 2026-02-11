# SignUpOutOrganisationSSResponse

OK

## Example Usage

```typescript
import { SignUpOutOrganisationSSResponse } from "crm/models/operations";

let value: SignUpOutOrganisationSSResponse = {
  exp: new Date("2022-03-10"),
  contact: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    firstName: "John",
    lastName: "Doe",
    isVerified: false,
    companyName: "Smith & Sons Ltd.",
  },
  organisations: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      type: "ORGANISATION",
      name: "CRMdotCOM",
    },
  ],
};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             | Example                                                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `accessToken`                                                                                                           | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `refreshToken`                                                                                                          | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `exp`                                                                                                                   | [Date](../../types/rfcdate.md)                                                                                          | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     | 2022-03-10                                                                                                              |
| `contact`                                                                                                               | [operations.SignUpOutOrganisationSSContact](../../models/operations/sign-up-out-organisation-ss-contact.md)             | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `organisations`                                                                                                         | [operations.SignUpOutOrganisationSSOrganisation](../../models/operations/sign-up-out-organisation-ss-organisation.md)[] | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |