# WalletFee

Details about the wallet fee related to the wallet journal transaction

## Example Usage

```typescript
import { WalletFee } from "crmcom/models/operations";

let value: WalletFee = {
  name: "1% on all wallet transactions",
};
```

## Fields

| Field                                                                                                                                                | Type                                                                                                                                                 | Required                                                                                                                                             | Description                                                                                                                                          | Example                                                                                                                                              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                                                                                                                                               | *string*                                                                                                                                             | :heavy_minus_sign:                                                                                                                                   | Defines the reason for which the fee was applied on wallet<br/> * `CREDIT` - On Credit Wallet Transactions<br/> * `DEBIT` - On Debit Wallet Transactions<br/> |                                                                                                                                                      |
| `name`                                                                                                                                               | *string*                                                                                                                                             | :heavy_minus_sign:                                                                                                                                   | The fee rule name                                                                                                                                    | 1% on all wallet transactions                                                                                                                        |