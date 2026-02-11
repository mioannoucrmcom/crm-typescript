# ComCrmWalletSelfServiceResourceGetTransactionsContent

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetTransactionsContent } from "crm/models/operations";

let value: ComCrmWalletSelfServiceResourceGetTransactionsContent = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  amount: 9.5,
  currency: "EUR",
  type: "CREDIT",
  postedOn: 1620912893,
  rewardEvent: {
    code: "123234342342432342324r43",
    amount: 14.99,
    spendMethod: "INSTANT",
    date: 1614954223,
    expiryDate: 1614954223,
    rewardOffer: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Birthday Offer",
    },
    performedBy: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Universal Name",
    },
  },
  financialEvent: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    number: "1234",
    referenceNumber: "REF12343",
    amount: 112.24,
    date: 1614954223,
  },
  walletFee: {
    name: "1% on all wallet transactions",
  },
  order: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    number: "ORD001",
    totalCost: 10.5,
    submittedOn: 1634282740,
    fulfilledBy: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "CRM",
    },
  },
  pocket: "BUSINESS_COMMERCE",
  exchangeRate: 0.97,
  totalDefaultCurrency: 0.97,
  defaultCurrencyCode: "EUR",
  walletExpiration: {
    date: 1614954223,
    commercePool: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Universal Name",
      description: "Sample description",
    },
  },
  transfer: {
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
  },
  blockedBy: {
    id: "3e3f2941-158f-411f-a0f0-a25d691b5853",
    entity: "PURCHASE",
    expirationDate: 1716239023,
  },
};
```

## Fields

| Field                                                                                                                                                                   | Type                                                                                                                                                                    | Required                                                                                                                                                                | Description                                                                                                                                                             | Example                                                                                                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                    | *string*                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                      | The entity identifier                                                                                                                                                   | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                    |
| `amount`                                                                                                                                                                | *number*                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                      | The wallet journal amount                                                                                                                                               | 9.5                                                                                                                                                                     |
| `currency`                                                                                                                                                              | *string*                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                      | The wallet’s journal currency                                                                                                                                           | EUR                                                                                                                                                                     |
| `type`                                                                                                                                                                  | [operations.ComCrmWalletSelfServiceResourceGetTransactionsContentType](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-content-type.md)   | :heavy_minus_sign:                                                                                                                                                      | The wallet journal type                                                                                                                                                 | CREDIT                                                                                                                                                                  |
| `postedOn`                                                                                                                                                              | *number*                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                      | The date that the wallet journal was posted                                                                                                                             | 1620912893                                                                                                                                                              |
| `rewardEvent`                                                                                                                                                           | [operations.RewardEvent](../../models/operations/reward-event.md)                                                                                                       | :heavy_minus_sign:                                                                                                                                                      | Details about the reward event related to the wallet journal transaction                                                                                                |                                                                                                                                                                         |
| `financialEvent`                                                                                                                                                        | [operations.FinancialEvent](../../models/operations/financial-event.md)                                                                                                 | :heavy_minus_sign:                                                                                                                                                      | Details about the financial event related to the wallet journal transaction                                                                                             |                                                                                                                                                                         |
| `walletFee`                                                                                                                                                             | [operations.WalletFee](../../models/operations/wallet-fee.md)                                                                                                           | :heavy_minus_sign:                                                                                                                                                      | Details about the wallet fee related to the wallet journal transaction                                                                                                  |                                                                                                                                                                         |
| `order`                                                                                                                                                                 | [operations.ComCrmWalletSelfServiceResourceGetTransactionsContentOrder](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-content-order.md) | :heavy_minus_sign:                                                                                                                                                      | Details about the order related to the wallet journal transaction                                                                                                       |                                                                                                                                                                         |
| `pocket`                                                                                                                                                                | [operations.PocketResponse](../../models/operations/pocket-response.md)                                                                                                 | :heavy_minus_sign:                                                                                                                                                      | Specifies which pocket the transaction was logged against. CRMCOM = CRM.COM pocket, BUSINESS = business open pocket, BUSINESS_COMMERCE = business commerce pocket       | BUSINESS_COMMERCE                                                                                                                                                       |
| `exchangeRate`                                                                                                                                                          | *number*                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                      | The exchange rate                                                                                                                                                       | 0.97                                                                                                                                                                    |
| `totalDefaultCurrency`                                                                                                                                                  | *number*                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                      | The total in default currency                                                                                                                                           | 0.97                                                                                                                                                                    |
| `defaultCurrencyCode`                                                                                                                                                   | *string*                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                      | The default currency code based on ISO 4217 standard                                                                                                                    | EUR                                                                                                                                                                     |
| `walletExpiration`                                                                                                                                                      | [operations.WalletExpiration](../../models/operations/wallet-expiration.md)                                                                                             | :heavy_minus_sign:                                                                                                                                                      | Details of expired Business Commerce funds                                                                                                                              |                                                                                                                                                                         |
| `transfer`                                                                                                                                                              | [operations.ComCrmWalletSelfServiceResourceGetTransactionsTransfer](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-transfer.md)          | :heavy_minus_sign:                                                                                                                                                      | Transfer transaction details                                                                                                                                            |                                                                                                                                                                         |
| `blockedBy`                                                                                                                                                             | [operations.BlockedBy](../../models/operations/blocked-by.md)                                                                                                           | :heavy_minus_sign:                                                                                                                                                      | The block details if the transaction is blocked                                                                                                                         |                                                                                                                                                                         |