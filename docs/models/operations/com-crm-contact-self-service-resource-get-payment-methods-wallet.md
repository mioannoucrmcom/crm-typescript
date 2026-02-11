# ComCrmContactSelfServiceResourceGetPaymentMethodsWallet

The wallet's main information. Required and applicable if the payment method type is WALLET

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetPaymentMethodsWallet } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceGetPaymentMethodsWallet = {
  phone: {
    countryCode: "CYP",
    number: "345678",
  },
  email: "jsmith@email.com",
  gatewayToken: [
    {
      gateway: "JCC",
      token: "Xt5EWLLDS7FJjR1c",
      integration: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                         | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   | Example                                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `phone`                                                                                                                                                                                       | [operations.ComCrmContactSelfServiceResourceGetPaymentMethodsPhone](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-phone.md)                               | :heavy_minus_sign:                                                                                                                                                                            | The phone used when registering to the walled-based payment method                                                                                                                            |                                                                                                                                                                                               |
| `email`                                                                                                                                                                                       | *string*                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                            | The email used when registering to the walled-based payment method                                                                                                                            | jsmith@email.com                                                                                                                                                                              |
| `gatewayToken`                                                                                                                                                                                | [operations.ComCrmContactSelfServiceResourceGetPaymentMethodsWalletGatewayToken](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-wallet-gateway-token.md)[] | :heavy_minus_sign:                                                                                                                                                                            | Details about the gateway related token was issued                                                                                                                                            |                                                                                                                                                                                               |