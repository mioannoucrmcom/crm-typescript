# ComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactionsResponse

OK

## Example Usage

```typescript
import {
  ComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactionsResponse,
} from "crmcom/models/operations";

let value:
  ComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactionsResponse =
    {
      content: [
        {
          rewardOffer: {
            id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
            name: "Universal Name",
          },
          amount: 9.23,
          currencyCode: "EUR",
          commercePool: {
            id: "a82c9cb5-a774-f30d-2d9e-aca7f0561751",
            name: "Coffee",
          },
          product: {
            id: "a82c9cb5-a774-f30d-2d9e-aca7f0561751",
            name: "Coffee",
          },
        },
      ],
    };
```

## Fields

| Field                                                                                                                                                                                                                        | Type                                                                                                                                                                                                                         | Required                                                                                                                                                                                                                     | Description                                                                                                                                                                                                                  |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `content`                                                                                                                                                                                                                    | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceGetPurchaseRewardTransactionsContent](../../models/operations/com-crm-purchase-customer-event-self-service-resource-get-purchase-reward-transactions-content.md)[] | :heavy_minus_sign:                                                                                                                                                                                                           | N/A                                                                                                                                                                                                                          |