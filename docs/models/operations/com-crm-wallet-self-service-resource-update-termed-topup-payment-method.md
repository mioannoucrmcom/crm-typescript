# ComCrmWalletSelfServiceResourceUpdateTermedTopupPaymentMethod

One of the wallet's payment methods that will be used in top-up

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceUpdateTermedTopupPaymentMethod } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceUpdateTermedTopupPaymentMethod = {
  type: "CARD",
  identity: {
    id: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
    identifier: "Visa *****1234 03/25",
  },
};
```

## Fields

| Field                                                                                                                                                       | Type                                                                                                                                                        | Required                                                                                                                                                    | Description                                                                                                                                                 | Example                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceUpdateTermedTopupType](../../models/operations/com-crm-wallet-self-service-resource-update-termed-topup-type.md) | :heavy_minus_sign:                                                                                                                                          | Payment method type                                                                                                                                         | CARD                                                                                                                                                        |
| `identity`                                                                                                                                                  | [operations.ComCrmWalletSelfServiceResourceUpdateIdentity](../../models/operations/com-crm-wallet-self-service-resource-update-identity.md)                 | :heavy_minus_sign:                                                                                                                                          | Payment method details                                                                                                                                      |                                                                                                                                                             |