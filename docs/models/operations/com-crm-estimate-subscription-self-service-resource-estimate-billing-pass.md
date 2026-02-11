# ComCrmEstimateSubscriptionSelfServiceResourceEstimateBillingPass

## Example Usage

```typescript
import { ComCrmEstimateSubscriptionSelfServiceResourceEstimateBillingPass } from "crmcom/models/operations";

let value: ComCrmEstimateSubscriptionSelfServiceResourceEstimateBillingPass = {
  code: "SLHY678993109PWE",
  pin: "1245",
};
```

## Fields

| Field                                                             | Type                                                              | Required                                                          | Description                                                       | Example                                                           |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `code`                                                            | *string*                                                          | :heavy_check_mark:                                                | The pass code                                                     | SLHY678993109PWE                                                  |
| `pin`                                                             | *string*                                                          | :heavy_minus_sign:                                                | The pass pin. Required only if the pass is assiociated with a pin | 1245                                                              |