# ComCrmWalletSelfServiceResourceGetTransactionsWallet

Details of the contact's wallet involved in the transfer transaction. If it's a 'debit' transfer, these details correspond to the receiving wallet, if it's a 'credit' transfer, these details relate to the sending wallet

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetTransactionsWallet } from "crm/models/operations";

let value: ComCrmWalletSelfServiceResourceGetTransactionsWallet = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  code: "2131424123",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `id`                                 | *string*                             | :heavy_minus_sign:                   | The entity identifier                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0 |
| `code`                               | *string*                             | :heavy_minus_sign:                   | The entity code                      | 2131424123                           |