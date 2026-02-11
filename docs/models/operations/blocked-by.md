# BlockedBy

The block details if the transaction is blocked

## Example Usage

```typescript
import { BlockedBy } from "crmcom/models/operations";

let value: BlockedBy = {
  id: "3e3f2941-158f-411f-a0f0-a25d691b5853",
  entity: "PURCHASE",
  expirationDate: 1716239023,
};
```

## Fields

| Field                                                                                                                                                      | Type                                                                                                                                                       | Required                                                                                                                                                   | Description                                                                                                                                                | Example                                                                                                                                                    |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                       | *string*                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                         | The identifier of the entity that blocked the item                                                                                                         | 3e3f2941-158f-411f-a0f0-a25d691b5853                                                                                                                       |
| `entity`                                                                                                                                                   | [operations.ComCrmWalletSelfServiceResourceGetTransactionsEntity](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-entity.md) | :heavy_minus_sign:                                                                                                                                         | The type of the entity that blocked the item                                                                                                               | PURCHASE                                                                                                                                                   |
| `expirationDate`                                                                                                                                           | *number*                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                         | The expiration date of the block                                                                                                                           | 1716239023                                                                                                                                                 |