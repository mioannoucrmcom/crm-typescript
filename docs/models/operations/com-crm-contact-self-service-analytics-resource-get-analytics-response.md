# ComCrmContactSelfServiceAnalyticsResourceGetAnalyticsResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceAnalyticsResourceGetAnalyticsResponse } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceAnalyticsResourceGetAnalyticsResponse = {
  totalOrders: 5,
  walletTotals: {
    totalTopUps: 3.2,
    totalSpent: 2.1,
    totalSent: 4,
    totalReceived: 5,
  },
  awardsPerMonth: [
    {
      amount: 2,
      timestamp: 1685566800,
    },
  ],
  redeemsPerMonth: [
    {
      amount: 2,
      timestamp: 1685566800,
    },
  ],
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  | Example                                                                      |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `totalOrders`                                                                | *number*                                                                     | :heavy_minus_sign:                                                           | The total orders performed by the contact                                    | 5                                                                            |
| `walletTotals`                                                               | [operations.WalletTotals](../../models/operations/wallet-totals.md)          | :heavy_minus_sign:                                                           | The total amounts for wallet transactions performed by the contact           |                                                                              |
| `awardsPerMonth`                                                             | [operations.AwardsPerMonth](../../models/operations/awards-per-month.md)[]   | :heavy_minus_sign:                                                           | The contact's award amount per month                                         |                                                                              |
| `redeemsPerMonth`                                                            | [operations.RedeemsPerMonth](../../models/operations/redeems-per-month.md)[] | :heavy_minus_sign:                                                           | The contact's redeem amount per month                                        |                                                                              |