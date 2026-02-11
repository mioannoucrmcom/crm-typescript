# ComCrmSettlementTransactionSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmSettlementTransactionSelfServiceResourceListResponse } from "crm/models/operations";

let value: ComCrmSettlementTransactionSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      settlementType: "AWARD",
      accountingType: "DEBIT",
      eventAmount: 2.22,
      settlementAmount: 20.12,
      fee: {
        feeType: "CONTRIBUTION",
        valueType: "AMOUNT",
        number: 2.84,
      },
      organisation: {
        id: "f2c2d9ea-5a94-729d-0c45-7fdd1d540e7b",
        name: "CRM",
      },
      settlementEvent: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        type: "PURCHASE",
        referenceNumber: "2833205645375343",
        amount: 102.79,
        postedDate: 1635170879,
      },
      rewardOffer: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "10% instant discount",
      },
      contact: {
        id: "f2c2d9ea-5a94-729d-0c45-7fdd1d540e7b",
        name: "George Paps",
        code: "4134213343214141",
      },
      schemeOwner: {
        id: "8720e95e-b22f-ffad-4d3d-d4f6b8e1d6e2",
        name: "CRM",
      },
      currencyCode: "EUR",
      exchangeRate: 0.97,
      totalDefaultCurrency: 0.97,
      defaultCurrencyCode: "EUR",
      isReverted: true,
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                  | Type                                                                                                                                                                   | Required                                                                                                                                                               | Description                                                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                               | [operations.ComCrmSettlementTransactionSelfServiceResourceListPaging](../../models/operations/com-crm-settlement-transaction-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                                                     | N/A                                                                                                                                                                    |
| `content`                                                                                                                                                              | [operations.ComCrmSettlementTransactionSelfServiceResourceListContent](../../models/operations/com-crm-settlement-transaction-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                                                     | N/A                                                                                                                                                                    |