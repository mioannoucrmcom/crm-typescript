# ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesRewards

Details about rewards due to purchase

## Example Usage

```typescript
import { ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesRewards } from "crm/models/operations";

let value: ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesRewards =
  {
    award: 121.99,
    spend: 12.22,
    redeem: 12.22,
  };
```

## Fields

| Field                           | Type                            | Required                        | Description                     | Example                         |
| ------------------------------- | ------------------------------- | ------------------------------- | ------------------------------- | ------------------------------- |
| `award`                         | *number*                        | :heavy_minus_sign:              | The total awarded amount        | 121.99                          |
| `spend`                         | *number*                        | :heavy_minus_sign:              | The total (actual) spent amount | 12.22                           |
| `redeem`                        | *number*                        | :heavy_minus_sign:              | The total redeemed amount       | 12.22                           |