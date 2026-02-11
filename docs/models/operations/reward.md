# Reward

Defines the supported rewards features

## Example Usage

```typescript
import { Reward } from "crmcom/models/operations";

let value: Reward = {
  tiering: true,
  preferredOrganisation: true,
  referFriend: {
    isSupported: true,
  },
  otpSpend: {
    isSupported: true,
    codeFormat: "BARCODE",
    spendAttributes: [
      {
        type: "AMOUNT",
      },
    ],
  },
  selfSubmitPurchases: {
    isSupported: true,
    selfSubmitMethods: [
      "BARCODE",
    ],
  },
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        | Example                                                                            |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `isSupported`                                                                      | *boolean*                                                                          | :heavy_minus_sign:                                                                 | Defines whether reward features should be available                                | false                                                                              |
| `tiering`                                                                          | *boolean*                                                                          | :heavy_minus_sign:                                                                 | Defines whether reward tiering will be supported                                   | true                                                                               |
| `preferredOrganisation`                                                            | *boolean*                                                                          | :heavy_minus_sign:                                                                 | Defines whether contact can select his/her preferred organisation for rewards      | true                                                                               |
| `referFriend`                                                                      | [operations.ReferFriend](../../models/operations/refer-friend.md)                  | :heavy_minus_sign:                                                                 | Defines the supported refer a friend features                                      | true                                                                               |
| `otpSpend`                                                                         | [operations.OtpSpend](../../models/operations/otp-spend.md)                        | :heavy_minus_sign:                                                                 | Defines the supported OTP spend features                                           | true                                                                               |
| `selfSubmitPurchases`                                                              | [operations.SelfSubmitPurchases](../../models/operations/self-submit-purchases.md) | :heavy_minus_sign:                                                                 | Defines the supported contact self-submit purchase events features                 | true                                                                               |