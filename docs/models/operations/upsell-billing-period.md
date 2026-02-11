# UpsellBillingPeriod

The billing period mapped to the specified price. Applicable only for termed and one-time services only.

## Example Usage

```typescript
import { UpsellBillingPeriod } from "crmcom/models/operations";

let value: UpsellBillingPeriod = {
  duration: 2,
  uot: "HOUR",
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   | Example                                                       |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `duration`                                                    | *number*                                                      | :heavy_minus_sign:                                            | Period Cycle duration                                         | 2                                                             |
| `uot`                                                         | [operations.UpsellUot](../../models/operations/upsell-uot.md) | :heavy_minus_sign:                                            | Period Cycle unit of time                                     | MONTHS                                                        |