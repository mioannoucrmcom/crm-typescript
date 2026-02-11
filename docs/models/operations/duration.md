# Duration

How long the offering will be applied. Applicable only when the offerring’s product is a termed service

## Example Usage

```typescript
import { Duration } from "crm/models/operations";

let value: Duration = {
  type: "PERIOD",
  period: {
    duration: 6,
    uot: "MONTH",
  },
  variableDiscounts: [
    {
      type: "PERCENT",
      amount: 1.99,
      period: {
        duration: 6,
        uot: "MONTH",
      },
      periodOrder: 1,
    },
  ],
};
```

## Fields

| Field                                                                                                                                                | Type                                                                                                                                                 | Required                                                                                                                                             | Description                                                                                                                                          | Example                                                                                                                                              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                                                                                                                                               | [operations.DurationType](../../models/operations/duration-type.md)                                                                                  | :heavy_check_mark:                                                                                                                                   | Indicates whether the offering will be applied once, for a period of time or forever.                                                                | PERIOD                                                                                                                                               |
| `period`                                                                                                                                             | [operations.ComCrmPromotionSelfServiceResourceGetSinglePeriod](../../models/operations/com-crm-promotion-self-service-resource-get-single-period.md) | :heavy_check_mark:                                                                                                                                   | Applicable and required only when the offering will be applied for a specific PERIOD                                                                 |                                                                                                                                                      |
| `variableDiscounts`                                                                                                                                  | [operations.VariableDiscount](../../models/operations/variable-discount.md)[]                                                                        | :heavy_minus_sign:                                                                                                                                   | Applicable only if the offering’s duration is set to VARIABLE_DISCOUNTS. At least one must be specified                                              |                                                                                                                                                      |