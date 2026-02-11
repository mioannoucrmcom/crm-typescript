# ComCrmWalletSelfServiceResourceGetTransactionsContact

Details of the contact involved in the transfer transaction. If it's a 'debit' transfer, these details pertain to the receiver contact, if it's a 'credit' transfer, these details relate to the sender contact

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetTransactionsContact } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceGetTransactionsContact = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Universal Name",
  code: "4134213343214141",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `id`                                 | *string*                             | :heavy_minus_sign:                   | The entity identifier                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0 |
| `name`                               | *string*                             | :heavy_minus_sign:                   | The entity name                      | Universal Name                       |
| `code`                               | *string*                             | :heavy_minus_sign:                   | The entity code                      | 4134213343214141                     |