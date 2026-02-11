# ComCrmPromotionSelfServiceResourceGetSinglePeriod

Applicable and required only when the offering will be applied for a specific PERIOD

## Example Usage

```typescript
import { ComCrmPromotionSelfServiceResourceGetSinglePeriod } from "crm/models/operations";

let value: ComCrmPromotionSelfServiceResourceGetSinglePeriod = {
  duration: 6,
  uot: "MONTH",
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   | Example                                                       |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `duration`                                                    | *number*                                                      | :heavy_check_mark:                                            | The period’s duration                                         | 6                                                             |
| `uot`                                                         | [operations.PeriodUot](../../models/operations/period-uot.md) | :heavy_check_mark:                                            | The period’s unit of time                                     | MONTH                                                         |