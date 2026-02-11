# VariableDiscount

## Example Usage

```typescript
import { VariableDiscount } from "crmcom/models/operations";

let value: VariableDiscount = {
  type: "PERCENT",
  amount: 1.99,
  period: {
    duration: 6,
    uot: "MONTH",
  },
  periodOrder: 1,
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              | Example                                                                                  |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `type`                                                                                   | [operations.VariableDiscountType](../../models/operations/variable-discount-type.md)     | :heavy_check_mark:                                                                       | Defines whether the offering is an actual discount amount or a discount percentage       |                                                                                          |
| `amount`                                                                                 | *number*                                                                                 | :heavy_check_mark:                                                                       | The discount amount or percentage depending on the offerring’s type                      | 1.99                                                                                     |
| `period`                                                                                 | [operations.VariableDiscountPeriod](../../models/operations/variable-discount-period.md) | :heavy_check_mark:                                                                       | Applicable and required only when the offering will be applied for a specific PERIOD     |                                                                                          |
| `periodOrder`                                                                            | *number*                                                                                 | :heavy_check_mark:                                                                       | Defines the discount order                                                               | 1                                                                                        |