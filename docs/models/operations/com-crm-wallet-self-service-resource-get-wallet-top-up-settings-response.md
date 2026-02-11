# ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsResponse

OK

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsResponse } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsResponse = {
  autoTopup: {
    threshold: 0.01,
    amount: 10.5,
    paymentMethod: {
      type: "CARD",
      identity: {
        id: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
        identifier: "Visa *****1234 03/25",
      },
    },
    currencyCode: "EUR",
  },
  termedTopup: {
    amount: 50,
    currencyCode: "EUR",
    frequency: "0 0 12 * * ?",
    paymentMethod: {
      type: "CARD",
      identity: {
        id: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
        identifier: "Visa *****1234 03/25",
      },
    },
    period: "MONTHLY",
  },
};
```

## Fields

| Field                                                                                                                                                                                  | Type                                                                                                                                                                                   | Required                                                                                                                                                                               | Description                                                                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `autoTopup`                                                                                                                                                                            | [operations.ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsAutoTopup](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-top-up-settings-auto-topup.md)     | :heavy_minus_sign:                                                                                                                                                                     | Automatically top up the wallet with an amount once a minimum threshold is reached, using one of the payment methods.                                                                  |
| `termedTopup`                                                                                                                                                                          | [operations.ComCrmWalletSelfServiceResourceGetWalletTopUpSettingsTermedTopup](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-top-up-settings-termed-topup.md) | :heavy_minus_sign:                                                                                                                                                                     | Top up the wallet on a frequent basis using one of the payment methods                                                                                                                 |