# ComCrmWalletSelfServiceResourceGetTransactionsResponse

OK

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetTransactionsResponse } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceGetTransactionsResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
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
    },
  ],
};
```

## Fields

| Field                                                                                                                                                          | Type                                                                                                                                                           | Required                                                                                                                                                       | Description                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                       | [operations.ComCrmWalletSelfServiceResourceGetTransactionsPaging](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-paging.md)     | :heavy_minus_sign:                                                                                                                                             | N/A                                                                                                                                                            |
| `content`                                                                                                                                                      | [operations.ComCrmWalletSelfServiceResourceGetTransactionsContent](../../models/operations/com-crm-wallet-self-service-resource-get-transactions-content.md)[] | :heavy_minus_sign:                                                                                                                                             | N/A                                                                                                                                                            |