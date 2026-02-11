# A2a

The account details.Required and applicable if the payment method is set to A2A

## Example Usage

```typescript
import { A2a } from "crmcom/models/operations";

let value: A2a = {
  schemeName: "BECSElectronicCredit",
  accountIdentification: "99-7354-1340583-01",
  currency: "NZD",
  accountName: "CurrentAccount",
  gatewayToken: [
    {
      gateway: "JCC",
      token: "Xt5EWLLDS7FJjR1c",
      integration: null,
    },
  ],
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  | Example                                                                      |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `schemeName`                                                                 | *string*                                                                     | :heavy_minus_sign:                                                           | The account scheme name                                                      | BECSElectronicCredit                                                         |
| `accountIdentification`                                                      | *string*                                                                     | :heavy_minus_sign:                                                           | The account identification                                                   | 99-7354-1340583-01                                                           |
| `currency`                                                                   | [operations.A2aCurrency](../../models/operations/a2a-currency.md)            | :heavy_minus_sign:                                                           | The account currency                                                         | NZD                                                                          |
| `accountName`                                                                | *string*                                                                     | :heavy_minus_sign:                                                           | The account name                                                             | CurrentAccount                                                               |
| `gatewayToken`                                                               | [operations.A2aGatewayToken](../../models/operations/a2a-gateway-token.md)[] | :heavy_minus_sign:                                                           | Details about the gateway related token was issued                           |                                                                              |