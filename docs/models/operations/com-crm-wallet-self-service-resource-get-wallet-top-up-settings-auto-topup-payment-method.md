# ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsAutoTopupPaymentMethod

One of the wallet's payment methods that will be used in automatic top-up

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsAutoTopupPaymentMethod } from "crm/models/operations";

let value:
  ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsAutoTopupPaymentMethod =
    {
      type: "CARD",
      identity: {
        id: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
        identifier: "Visa *****1234 03/25",
      },
    };
```

## Fields

| Field                                                                                                                                                                                       | Type                                                                                                                                                                                        | Required                                                                                                                                                                                    | Description                                                                                                                                                                                 | Example                                                                                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsAutoTopupType](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-top-up-settings-auto-topup-type.md) | :heavy_minus_sign:                                                                                                                                                                          | Payment method type                                                                                                                                                                         | CARD                                                                                                                                                                                        |
| `identity`                                                                                                                                                                                  | [operations.AutoTopupIdentity](../../models/operations/auto-topup-identity.md)                                                                                                              | :heavy_minus_sign:                                                                                                                                                                          | Payment method details                                                                                                                                                                      |                                                                                                                                                                                             |