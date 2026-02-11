# Merchant

The merchant features that will be supported by the application

## Example Usage

```typescript
import { Merchant } from "crm/models/operations";

let value: Merchant = {
  purchase: {
    manualSpend: true,
    automaticSpend: true,
    spendFullPurchaseAmount: true,
    restrictFullyCovered: true,
  },
};
```

## Fields

| Field                                                                                                                                                                  | Type                                                                                                                                                                   | Required                                                                                                                                                               | Description                                                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `purchase`                                                                                                                                                             | [operations.ComCrmApplicationSelfServiceResourceGetApplicationPurchase](../../models/operations/com-crm-application-self-service-resource-get-application-purchase.md) | :heavy_minus_sign:                                                                                                                                                     | Defines the supported purchase event features                                                                                                                          |