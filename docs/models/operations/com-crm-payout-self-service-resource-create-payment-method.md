# ComCrmPayoutSelfServiceResourceCreatePaymentMethod

The payment method that will be used to return back money to the contact

## Example Usage

```typescript
import { ComCrmPayoutSelfServiceResourceCreatePaymentMethod } from "crm/models/operations";

let value: ComCrmPayoutSelfServiceResourceCreatePaymentMethod = {
  id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
  type: "CARD",
};
```

## Fields

| Field                                                                                                                                                              | Type                                                                                                                                                               | Required                                                                                                                                                           | Description                                                                                                                                                        | Example                                                                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                               | *string*                                                                                                                                                           | :heavy_check_mark:                                                                                                                                                 | The unique identifier of the contac'ts payment method. Applicable and required when the select payment method type is either a Card, an Account Debit or a Wallet. | CAD1E31269B76D7A65ACCE45B2E68DFD                                                                                                                                   |
| `type`                                                                                                                                                             | [operations.ComCrmPayoutSelfServiceResourceCreateType](../../models/operations/com-crm-payout-self-service-resource-create-type.md)                                | :heavy_check_mark:                                                                                                                                                 | Available payment method types                                                                                                                                     |                                                                                                                                                                    |