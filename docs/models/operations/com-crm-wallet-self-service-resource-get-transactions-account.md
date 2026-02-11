# ComCrmWalletSelfServiceResourceGetTransactionsAccount

Details of the contact's account involved in the transfer transaction. If it's a 'debit' transfer, these details correspond to the receiving account, if it's a 'credit' transfer, these details relate to the sending account

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetTransactionsAccount } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceGetTransactionsAccount = {};
```

## Fields

| Field                 | Type                  | Required              | Description           |
| --------------------- | --------------------- | --------------------- | --------------------- |
| `id`                  | *string*              | :heavy_minus_sign:    | the entity identifier |
| `number`              | *string*              | :heavy_minus_sign:    | the entity number     |