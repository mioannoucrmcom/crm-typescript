# ComCrmContactSelfServiceResourceAddPaymentMethodWalletGatewayToken

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceAddPaymentMethodWalletGatewayToken } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceAddPaymentMethodWalletGatewayToken =
  {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    gateway: "JCC",
    token: "Xt5EWLLDS7FJjR1c",
    alternativeToken: "Xt5EWLLDS7FJjR1c",
    integrationId: "bce504a4-f712-5262-183c-f58218a7a0ed",
  };
```

## Fields

| Field                                                                 | Type                                                                  | Required                                                              | Description                                                           | Example                                                               |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `id`                                                                  | *string*                                                              | :heavy_minus_sign:                                                    | The entity identifier that will be created                            | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                  |
| `gateway`                                                             | [operations.WalletGateway](../../models/operations/wallet-gateway.md) | :heavy_minus_sign:                                                    | Defines the gateway that issued such token                            | JCC                                                                   |
| `token`                                                               | *string*                                                              | :heavy_check_mark:                                                    | The card related token                                                | Xt5EWLLDS7FJjR1c                                                      |
| `alternativeToken`                                                    | *string*                                                              | :heavy_minus_sign:                                                    | An alternative token for the card                                     | Xt5EWLLDS7FJjR1c                                                      |
| `integrationId`                                                       | *string*                                                              | :heavy_minus_sign:                                                    | The gateway integration (identifier)                                  | bce504a4-f712-5262-183c-f58218a7a0ed                                  |