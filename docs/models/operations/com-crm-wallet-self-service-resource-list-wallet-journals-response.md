# ComCrmWalletSelfServiceResourceListWalletJournalsResponse

OK

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceListWalletJournalsResponse } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceListWalletJournalsResponse = {
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
      expirationDate: 1620912893,
      unallocatedAmount: 9.5,
      description: "Posted for purchase",
      exchangeRate: 0.97,
      totalDefaultCurrency: 0.97,
      defaultCurrencyCode: "EUR",
      transactionType: "SETTLEMENT_PROCESS",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                 | Type                                                                                                                                                                  | Required                                                                                                                                                              | Description                                                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                              | [operations.ComCrmWalletSelfServiceResourceListWalletJournalsPaging](../../models/operations/com-crm-wallet-self-service-resource-list-wallet-journals-paging.md)     | :heavy_minus_sign:                                                                                                                                                    | N/A                                                                                                                                                                   |
| `content`                                                                                                                                                             | [operations.ComCrmWalletSelfServiceResourceListWalletJournalsContent](../../models/operations/com-crm-wallet-self-service-resource-list-wallet-journals-content.md)[] | :heavy_minus_sign:                                                                                                                                                    | N/A                                                                                                                                                                   |