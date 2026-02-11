# VariableDiscountPeriod

Applicable and required only when the offering will be applied for a specific PERIOD

## Example Usage

```typescript
import { VariableDiscountPeriod } from "crmcom/models/operations";

let value: VariableDiscountPeriod = {
  duration: 6,
  uot: "MONTH",
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        | Example                                                                            |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `duration`                                                                         | *number*                                                                           | :heavy_check_mark:                                                                 | The period’s duration                                                              | 6                                                                                  |
| `uot`                                                                              | [operations.VariableDiscountUot](../../models/operations/variable-discount-uot.md) | :heavy_check_mark:                                                                 | The period’s unit of time                                                          | MONTH                                                                              |