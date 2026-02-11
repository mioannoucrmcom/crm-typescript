# ComCrmContactSelfServiceResourceUpdatePaymentMethodCard

Applicable only when updating a payment method of type Card

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceUpdatePaymentMethodCard } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceUpdatePaymentMethodCard = {
  expMonth: 2,
  expYear: 2022,
  alternativeToken: "Xt5EWLLDS7FJjR1c",
  integrationId: "bce504a4-f712-5262-183c-f58218a7a0ed",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `expMonth`                           | *number*                             | :heavy_check_mark:                   | The card expiration month            | 2                                    |
| `expYear`                            | *number*                             | :heavy_check_mark:                   | The card expiration year             | 2022                                 |
| `alternativeToken`                   | *string*                             | :heavy_minus_sign:                   | The card alternative token           | Xt5EWLLDS7FJjR1c                     |
| `integrationId`                      | *string*                             | :heavy_minus_sign:                   | The gateway integration (identifier) | bce504a4-f712-5262-183c-f58218a7a0ed |