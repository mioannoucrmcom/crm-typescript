# ComCrmWalletSelfServiceResourceGetWalletSummarisedTotalsResponse

OK

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetWalletSummarisedTotalsResponse } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceGetWalletSummarisedTotalsResponse = {
  walletTotals: [
    {
      type: "TOP_UP",
      total: 100.5,
      currencyCode: "EUR",
    },
  ],
};
```

## Fields

| Field                                                               | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `walletTotals`                                                      | [operations.WalletTotal](../../models/operations/wallet-total.md)[] | :heavy_minus_sign:                                                  | N/A                                                                 |