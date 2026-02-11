# ComCrmWalletSelfServiceResourceRequestOTPIdentity

The CRM.COM Wallet's identity

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceRequestOTPIdentity } from "crm/models/operations";

let value: ComCrmWalletSelfServiceResourceRequestOTPIdentity = {
  type: "EMAIL",
  value: "e_kwsta@crm.com",
  countryCode: "CYP",
};
```

## Fields

| Field                                                                                                                                                       | Type                                                                                                                                                        | Required                                                                                                                                                    | Description                                                                                                                                                 | Example                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceRequestOTPType](../../models/operations/com-crm-wallet-self-service-resource-request-otp-type.md)                | :heavy_check_mark:                                                                                                                                          | A contact's wallet can either be identified across the business network based on a contact's phone or email address                                         | EMAIL                                                                                                                                                       |
| `value`                                                                                                                                                     | *string*                                                                                                                                                    | :heavy_check_mark:                                                                                                                                          | The contact's phone or email address depending on the identity's type                                                                                       | e_kwsta@crm.com                                                                                                                                             |
| `countryCode`                                                                                                                                               | [operations.ComCrmWalletSelfServiceResourceRequestOTPCountryCode](../../models/operations/com-crm-wallet-self-service-resource-request-otp-country-code.md) | :heavy_minus_sign:                                                                                                                                          | 3-character phone number country code based on ISO 3166                                                                                                     | CYP                                                                                                                                                         |