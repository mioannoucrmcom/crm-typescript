# ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesFees

Details about applied fees due to purchase's rewards

## Example Usage

```typescript
import { ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesFees } from "crmcom/models/operations";

let value: ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesFees = {
  total: 2.54,
  creditFee: 1.21,
  debitFee: 1.34,
};
```

## Fields

| Field                                              | Type                                               | Required                                           | Description                                        | Example                                            |
| -------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------- |
| `total`                                            | *number*                                           | :heavy_minus_sign:                                 | The total fee amount (sum of all fee amounts)      | 2.54                                               |
| `creditFee`                                        | *number*                                           | :heavy_minus_sign:                                 | The fee that was applied on awards (credit wallet) | 1.21                                               |
| `debitFee`                                         | *number*                                           | :heavy_minus_sign:                                 | The fee that was applied on spends (debit wallet)  | 1.34                                               |