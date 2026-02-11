# Credential

## Example Usage

```typescript
import { Credential } from "crmcom/models/operations";

let value: Credential = {
  name: "BIRTHDATE",
  value: "1234567",
  giftPass: {
    email: "jonf.doe@gmail.com",
    phone: {
      number: "99000000",
      countryCode: "CYP",
    },
    pin: "132435",
    lastSpendAmount: 2.5,
  },
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 | Example                                                                     |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `name`                                                                      | [operations.Name](../../models/operations/name.md)                          | :heavy_check_mark:                                                          | The predetermined information that will be used to identify the contact     | BIRTHDATE                                                                   |
| `value`                                                                     | *string*                                                                    | :heavy_check_mark:                                                          | The value of the credential to check                                        | 1234567                                                                     |
| `giftPass`                                                                  | [operations.GiftPass](../../models/operations/gift-pass.md)                 | :heavy_minus_sign:                                                          | The gift pass information to check (applicable only if type is “GIFT_PASS”) |                                                                             |