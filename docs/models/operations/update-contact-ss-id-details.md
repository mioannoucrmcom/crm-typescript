# UpdateContactSSIdDetails

Contact’s ID information

## Example Usage

```typescript
import { UpdateContactSSIdDetails } from "crmcom/models/operations";

let value: UpdateContactSSIdDetails = {
  number: "809251833",
  issuingCountryCode: "CYP",
  expirationDate: 1709295528,
};
```

## Fields

| Field                                                                                                                                 | Type                                                                                                                                  | Required                                                                                                                              | Description                                                                                                                           | Example                                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| `number`                                                                                                                              | *string*                                                                                                                              | :heavy_check_mark:                                                                                                                    | ID number                                                                                                                             | 809251833                                                                                                                             |
| `issuingCountryCode`                                                                                                                  | [operations.UpdateContactSSIdDetailsIssuingCountryCode](../../models/operations/update-contact-ss-id-details-issuing-country-code.md) | :heavy_check_mark:                                                                                                                    | 3-character country code based on ISO 3166                                                                                            | CYP                                                                                                                                   |
| `expirationDate`                                                                                                                      | *number*                                                                                                                              | :heavy_check_mark:                                                                                                                    | ID’s expiry date                                                                                                                      | 1709295528                                                                                                                            |