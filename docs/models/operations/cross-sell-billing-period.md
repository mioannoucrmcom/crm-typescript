# CrossSellBillingPeriod

The billing period mapped to the specified price. Applicable only for termed and one-time services only.

## Example Usage

```typescript
import { CrossSellBillingPeriod } from "crm/models/operations";

let value: CrossSellBillingPeriod = {
  duration: 2,
  uot: "WEEK",
};
```

## Fields

| Field                                                                | Type                                                                 | Required                                                             | Description                                                          | Example                                                              |
| -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| `duration`                                                           | *number*                                                             | :heavy_minus_sign:                                                   | Period Cycle duration                                                | 2                                                                    |
| `uot`                                                                | [operations.CrossSellUot](../../models/operations/cross-sell-uot.md) | :heavy_minus_sign:                                                   | Period Cycle unit of time                                            | MONTHS                                                               |