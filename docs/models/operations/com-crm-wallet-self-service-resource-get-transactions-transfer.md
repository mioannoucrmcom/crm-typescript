# ComCrmWalletSelfServiceResourceGetTransactionsTransfer

Transfer transaction details

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetTransactionsTransfer } from "crm/models/operations";

let value: ComCrmWalletSelfServiceResourceGetTransactionsTransfer = {
  contact: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "Universal Name",
    code: "4134213343214141",
  },
  commercePool: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Universal Name",
  },
  wallet: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    code: "2131424123",
  },
};
```

## Fields

| Field                                                                                                                                                                                                                          | Type                                                                                                                                                                                                                           | Required                                                                                                                                                                                                                       | Description                                                                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `contact`                                                                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceGetTransactionsContact](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-contact.md)                                                                   | :heavy_minus_sign:                                                                                                                                                                                                             | Details of the contact involved in the transfer transaction. If it's a 'debit' transfer, these details pertain to the receiver contact, if it's a 'credit' transfer, these details relate to the sender contact                |
| `commercePool`                                                                                                                                                                                                                 | [operations.ComCrmWalletSelfServiceResourceGetTransactionsTransferCommercePool](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-transfer-commerce-pool.md)                                       | :heavy_minus_sign:                                                                                                                                                                                                             | If the transfer includes spending conditions, then the commerce pool details are provided too. Applicable only for transfers to the Business Commerce Pocket.                                                                  |
| `wallet`                                                                                                                                                                                                                       | [operations.ComCrmWalletSelfServiceResourceGetTransactionsWallet](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-wallet.md)                                                                     | :heavy_minus_sign:                                                                                                                                                                                                             | Details of the contact's wallet involved in the transfer transaction. If it's a 'debit' transfer, these details correspond to the receiving wallet, if it's a 'credit' transfer, these details relate to the sending wallet    |
| `account`                                                                                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceGetTransactionsAccount](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-account.md)                                                                   | :heavy_minus_sign:                                                                                                                                                                                                             | Details of the contact's account involved in the transfer transaction. If it's a 'debit' transfer, these details correspond to the receiving account, if it's a 'credit' transfer, these details relate to the sending account |