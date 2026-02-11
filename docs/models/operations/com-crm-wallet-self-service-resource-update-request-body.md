# ComCrmWalletSelfServiceResourceUpdateRequestBody

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceUpdateRequestBody } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceUpdateRequestBody = {
  autoTopup: {
    threshold: 0,
    amount: 50,
    paymentMethod: {
      id: "a68cfe78-153d-e7ad-a4b4-4d783f7e6219",
      type: "CARD",
      identifier: "Visa *****1234 03/25",
    },
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

| Field                                                                                                                                              | Type                                                                                                                                               | Required                                                                                                                                           | Description                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| `autoTopup`                                                                                                                                        | [operations.ComCrmWalletSelfServiceResourceUpdateAutoTopup](../../models/operations/com-crm-wallet-self-service-resource-update-auto-topup.md)     | :heavy_minus_sign:                                                                                                                                 | Contacts determine when their wallet will be automatically topped-up using one of their payment method                                             |
| `termedTopup`                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceUpdateTermedTopup](../../models/operations/com-crm-wallet-self-service-resource-update-termed-topup.md) | :heavy_minus_sign:                                                                                                                                 | Contacts define how often their wallet will be automatically topped-up.                                                                            |