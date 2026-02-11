# GiftPass

The gift pass information to check (applicable only if type is “GIFT_PASS”)

## Example Usage

```typescript
import { GiftPass } from "crm/models/operations";

let value: GiftPass = {
  email: "jonf.doe@gmail.com",
  phone: {
    number: "99000000",
    countryCode: "CYP",
  },
  pin: "132435",
  lastSpendAmount: 2.5,
};
```

## Fields

| Field                                                                                                                                            | Type                                                                                                                                             | Required                                                                                                                                         | Description                                                                                                                                      | Example                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| `email`                                                                                                                                          | *string*                                                                                                                                         | :heavy_minus_sign:                                                                                                                               | The email address that will receive the one-time-password (email or phone must be provided)                                                      | jonf.doe@gmail.com                                                                                                                               |
| `phone`                                                                                                                                          | [operations.ComCrmContactSelfServiceResourceRequestOTPPhone](../../models/operations/com-crm-contact-self-service-resource-request-otp-phone.md) | :heavy_minus_sign:                                                                                                                               | The contact’s phone                                                                                                                              |                                                                                                                                                  |
| `pin`                                                                                                                                            | *string*                                                                                                                                         | :heavy_minus_sign:                                                                                                                               | The gift pass pin (pin or last_spend_amount must be provided)                                                                                    | 132435                                                                                                                                           |
| `lastSpendAmount`                                                                                                                                | *number*                                                                                                                                         | :heavy_minus_sign:                                                                                                                               | The last spend amount performed, semi-optional - either pin or last_spend_amount must be provided                                                | 2.5                                                                                                                                              |