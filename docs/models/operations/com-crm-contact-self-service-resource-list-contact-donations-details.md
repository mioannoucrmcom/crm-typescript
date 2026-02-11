# ComCrmContactSelfServiceResourceListContactDonationsDetails

The donation's details that show how/when donations are made by the contact

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceListContactDonationsDetails } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceListContactDonationsDetails = {
  multiplier: 2,
  amount: 2,
};
```

## Fields

| Field                                                                                                                                        | Type                                                                                                                                         | Required                                                                                                                                     | Description                                                                                                                                  | Example                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| `multiplier`                                                                                                                                 | *number*                                                                                                                                     | :heavy_minus_sign:                                                                                                                           | Applicable for donations per transaction. The donations amount is calculated based on the purchase's rounded up amount times this multipler. | 2                                                                                                                                            |
| `amount`                                                                                                                                     | *number*                                                                                                                                     | :heavy_minus_sign:                                                                                                                           | Applicable for recurring donations wutg variable amount.                                                                                     | 2                                                                                                                                            |