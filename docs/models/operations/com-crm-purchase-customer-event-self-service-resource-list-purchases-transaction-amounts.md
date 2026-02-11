# ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesTransactionAmounts

The total transaction amounts of a purchase

## Example Usage

```typescript
import { ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesTransactionAmounts } from "crm/models/operations";

let value:
  ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesTransactionAmounts =
    {
      net: 12.11,
      tax: 0.11,
      discount: 1,
      total: 11,
    };
```

## Fields

| Field                        | Type                         | Required                     | Description                  | Example                      |
| ---------------------------- | ---------------------------- | ---------------------------- | ---------------------------- | ---------------------------- |
| `net`                        | *number*                     | :heavy_check_mark:           | The net amount               | 12.11                        |
| `tax`                        | *number*                     | :heavy_check_mark:           | The tax amount               | 0.11                         |
| `discount`                   | *number*                     | :heavy_minus_sign:           | The discount amount          | 1                            |
| `total`                      | *number*                     | :heavy_check_mark:           | The total amount (net + tax) | 11                           |