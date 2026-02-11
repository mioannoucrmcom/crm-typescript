# GetSingleContactSSIdDetails

Contact’s ID information

## Example Usage

```typescript
import { GetSingleContactSSIdDetails } from "crm/models/operations";

let value: GetSingleContactSSIdDetails = {
  number: "809251833",
  issuingCountryCode: "CYP",
  expirationDate: 1677673128,
};
```

## Fields

| Field                                                                                                                                        | Type                                                                                                                                         | Required                                                                                                                                     | Description                                                                                                                                  | Example                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| `number`                                                                                                                                     | *string*                                                                                                                                     | :heavy_minus_sign:                                                                                                                           | ID number                                                                                                                                    | 809251833                                                                                                                                    |
| `issuingCountryCode`                                                                                                                         | [operations.GetSingleContactSSIdDetailsIssuingCountryCode](../../models/operations/get-single-contact-ss-id-details-issuing-country-code.md) | :heavy_minus_sign:                                                                                                                           | Country code where id was issued. 3-letter ISO 3166-1 country code.                                                                          | CYP                                                                                                                                          |
| `expirationDate`                                                                                                                             | *number*                                                                                                                                     | :heavy_minus_sign:                                                                                                                           | Id’s expiry date                                                                                                                             | 1677673128                                                                                                                                   |