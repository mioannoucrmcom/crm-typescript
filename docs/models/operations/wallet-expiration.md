# WalletExpiration

Details of expired Business Commerce funds

## Example Usage

```typescript
import { WalletExpiration } from "crmcom/models/operations";

let value: WalletExpiration = {
  date: 1614954223,
  commercePool: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Universal Name",
    description: "Sample description",
  },
};
```

## Fields

| Field                                                                                                 | Type                                                                                                  | Required                                                                                              | Description                                                                                           | Example                                                                                               |
| ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `date`                                                                                                | *number*                                                                                              | :heavy_minus_sign:                                                                                    | Expiry date of Commerce funds                                                                         | 1614954223                                                                                            |
| `commercePool`                                                                                        | [operations.WalletExpirationCommercePool](../../models/operations/wallet-expiration-commerce-pool.md) | :heavy_minus_sign:                                                                                    | Details of Commerce Pool                                                                              |                                                                                                       |