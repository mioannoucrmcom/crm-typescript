# ComCrmContactSelfServiceResourceAddPaymentMethodWallet

The phone details (required and applicable if the payment method is set to PHONE)

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceAddPaymentMethodWallet } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceAddPaymentMethodWallet = {
  phoneDetails: {
    countryCode: "CYP",
    number: "345678",
  },
  email: "jsmith@email.com",
  name: "John Smith",
  gatewayToken: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      gateway: "JCC",
      token: "Xt5EWLLDS7FJjR1c",
      alternativeToken: "Xt5EWLLDS7FJjR1c",
      integrationId: "bce504a4-f712-5262-183c-f58218a7a0ed",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                       | Type                                                                                                                                                                                        | Required                                                                                                                                                                                    | Description                                                                                                                                                                                 | Example                                                                                                                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `phoneDetails`                                                                                                                                                                              | [operations.PhoneDetails](../../models/operations/phone-details.md)                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                          | The phone used when registering to the walled-based payment method                                                                                                                          |                                                                                                                                                                                             |
| `email`                                                                                                                                                                                     | *string*                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                          | The email used when registering to the walled-based payment method                                                                                                                          | jsmith@email.com                                                                                                                                                                            |
| `name`                                                                                                                                                                                      | *string*                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                          | The name used when registering to the walled-based payment method eg. The name of the revolut account                                                                                       | John Smith                                                                                                                                                                                  |
| `gatewayToken`                                                                                                                                                                              | [operations.ComCrmContactSelfServiceResourceAddPaymentMethodWalletGatewayToken](../../models/operations/com-crm-contact-self-service-resource-add-payment-method-wallet-gateway-token.md)[] | :heavy_minus_sign:                                                                                                                                                                          | Details about the gateway related token was issued                                                                                                                                          |                                                                                                                                                                                             |