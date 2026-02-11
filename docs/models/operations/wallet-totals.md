# WalletTotals

The total amounts for wallet transactions performed by the contact

## Example Usage

```typescript
import { WalletTotals } from "crmcom/models/operations";

let value: WalletTotals = {
  totalTopUps: 3.2,
  totalSpent: 2.1,
  totalSent: 4,
  totalReceived: 5,
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         | Example                                                                             |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `totalTopUps`                                                                       | *number*                                                                            | :heavy_minus_sign:                                                                  | The total top-up amount                                                             | 3.2                                                                                 |
| `totalSpent`                                                                        | *number*                                                                            | :heavy_minus_sign:                                                                  | The total spent amount                                                              | 2.1                                                                                 |
| `totalSent`                                                                         | *number*                                                                            | :heavy_minus_sign:                                                                  | The total amount that sent from this contact (result of a transfer transaction)     | 4                                                                                   |
| `totalReceived`                                                                     | *number*                                                                            | :heavy_minus_sign:                                                                  | The total amount that received from this contact (result of a transfer transaction) | 5                                                                                   |