# ComCrmWalletSelfServiceResourceGetWalletLimitsResponse

OK

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetWalletLimitsResponse } from "crmcom/models/operations";

let value: ComCrmWalletSelfServiceResourceGetWalletLimitsResponse = {
  limitRules: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Monthly Limits for VIP",
      maximumNumber: 50,
      maximumAmount: 200,
      appliesFor: [
        "DEBIT",
      ],
      currencyCode: "EUR",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                | Type                                                                                                                                                                 | Required                                                                                                                                                             | Description                                                                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `limitRules`                                                                                                                                                         | [operations.ComCrmWalletSelfServiceResourceGetWalletLimitsLimitRule](../../models/operations/com-crm-wallet-self-service-resource-get-wallet-limits-limit-rule.md)[] | :heavy_minus_sign:                                                                                                                                                   | N/A                                                                                                                                                                  |