# UseWalletFunds

Defines whether contact can pay for order using wallet funds

## Example Usage

```typescript
import { UseWalletFunds } from "crmcom/models/operations";

let value: UseWalletFunds = {
  specificFundsAmount: false,
  coverFullBasket: false,
};
```

## Fields

| Field                                                                          | Type                                                                           | Required                                                                       | Description                                                                    | Example                                                                        |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| `isSupported`                                                                  | *boolean*                                                                      | :heavy_minus_sign:                                                             | Defines whether contact can pay for order using wallet funds                   | false                                                                          |
| `specificFundsAmount`                                                          | *boolean*                                                                      | :heavy_minus_sign:                                                             | Defines whether contacts can specific the wallet funds amount to use on orders | false                                                                          |
| `coverFullBasket`                                                              | *boolean*                                                                      | :heavy_minus_sign:                                                             | Defines whether the wallet fund amount must cover the full basket amount       | false                                                                          |