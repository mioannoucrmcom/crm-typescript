# ComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchaseTransactionAmounts

Details about the purchase transaction amounts

## Example Usage

```typescript
import {
  ComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchaseTransactionAmounts,
} from "crmcom/models/operations";

let value:
  ComCrmPurchaseCustomerEventSelfServiceResourceGetSinglePurchaseTransactionAmounts =
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
| `net`                        | *number*                     | :heavy_minus_sign:           | The net amount               | 12.11                        |
| `tax`                        | *number*                     | :heavy_minus_sign:           | The tax amount               | 0.11                         |
| `discount`                   | *number*                     | :heavy_minus_sign:           | The discount amount          | 1                            |
| `total`                      | *number*                     | :heavy_minus_sign:           | The total amount (net + tax) | 11                           |