# ComCrmWalletSelfServiceResourceUpdateAutoTopup

Contacts determine when their wallet will be automatically topped-up using one of their payment method

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceUpdateAutoTopup } from "crm/models/operations";

let value: ComCrmWalletSelfServiceResourceUpdateAutoTopup = {
  threshold: 0,
  amount: 50,
  paymentMethod: {
    id: "a68cfe78-153d-e7ad-a4b4-4d783f7e6219",
    type: "CARD",
    identifier: "Visa *****1234 03/25",
  },
};
```

## Fields

| Field                                                                                                                                                                      | Type                                                                                                                                                                       | Required                                                                                                                                                                   | Description                                                                                                                                                                | Example                                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `threshold`                                                                                                                                                                | *number*                                                                                                                                                                   | :heavy_check_mark:                                                                                                                                                         | The minimum wallet business open balance at which the auto-top up will be triggered                                                                                        | 0                                                                                                                                                                          |
| `amount`                                                                                                                                                                   | *number*                                                                                                                                                                   | :heavy_check_mark:                                                                                                                                                         | The top-up's amount                                                                                                                                                        | 50                                                                                                                                                                         |
| `paymentMethod`                                                                                                                                                            | [operations.ComCrmWalletSelfServiceResourceUpdateAutoTopupPaymentMethod](../../models/operations/com-crm-wallet-self-service-resource-update-auto-topup-payment-method.md) | :heavy_check_mark:                                                                                                                                                         | One of the wallet's payment methods that will be used in top-up                                                                                                            |                                                                                                                                                                            |