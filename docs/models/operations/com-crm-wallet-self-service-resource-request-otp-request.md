# ComCrmWalletSelfServiceResourceRequestOTPRequest

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceRequestOTPRequest } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceRequestOTPRequest = {
  identity: {
    type: "EMAIL",
    value: "e_kwsta@crm.com",
    countryCode: "CYP",
  },
};
```

## Fields

| Field                                                                                                                                                | Type                                                                                                                                                 | Required                                                                                                                                             | Description                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| `identity`                                                                                                                                           | [operations.ComCrmWalletSelfServiceResourceRequestOTPIdentity](../../models/operations/com-crm-wallet-self-service-resource-request-otp-identity.md) | :heavy_minus_sign:                                                                                                                                   | The CRM.COM Wallet's identity                                                                                                                        |