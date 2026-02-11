# OtpSpend

Defines the supported OTP spend features

## Example Usage

```typescript
import { OtpSpend } from "crm/models/operations";

let value: OtpSpend = {
  isSupported: true,
  codeFormat: "BARCODE",
  spendAttributes: [
    {
      type: "AMOUNT",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                       | Type                                                                                                                                                                        | Required                                                                                                                                                                    | Description                                                                                                                                                                 | Example                                                                                                                                                                     |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `isSupported`                                                                                                                                                               | *boolean*                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                          | Defines whether OTP spend will be supported                                                                                                                                 | true                                                                                                                                                                        |
| `codeFormat`                                                                                                                                                                | [operations.ComCrmApplicationSelfServiceResourceGetApplicationCodeFormat](../../models/operations/com-crm-application-self-service-resource-get-application-code-format.md) | :heavy_minus_sign:                                                                                                                                                          | The alternative token code format. This code can be in the form of a barcode or QR code                                                                                     | BARCODE                                                                                                                                                                     |
| `spendAttributes`                                                                                                                                                           | [operations.SpendAttribute](../../models/operations/spend-attribute.md)[]                                                                                                   | :heavy_minus_sign:                                                                                                                                                          | Defines the supplementary attributes that will be supported for OTP spends (required when OTP spend is enabled)                                                             |                                                                                                                                                                             |