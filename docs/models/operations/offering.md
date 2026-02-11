# Offering

## Example Usage

```typescript
import { Offering } from "crmcom/models/operations";

let value: Offering = {
  product: {
    itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
    name: "HD STB",
    sku: "STB12345",
  },
  amount: 1.99,
  duration: {
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
  },
};
```

## Fields

| Field                                                                                                   | Type                                                                                                    | Required                                                                                                | Description                                                                                             | Example                                                                                                 |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| `product`                                                                                               | [operations.OfferingProduct](../../models/operations/offering-product.md)                               | :heavy_minus_sign:                                                                                      | The product on which the discount will be applied                                                       |                                                                                                         |
| `type`                                                                                                  | [operations.OfferingType](../../models/operations/offering-type.md)                                     | :heavy_minus_sign:                                                                                      | Defines whether the offering is an actual discount amount or a discount percentage                      |                                                                                                         |
| `amount`                                                                                                | *number*                                                                                                | :heavy_minus_sign:                                                                                      | The discount amount or percentage depending on the offerring’s type                                     | 1.99                                                                                                    |
| `duration`                                                                                              | [operations.Duration](../../models/operations/duration.md)                                              | :heavy_minus_sign:                                                                                      | How long the offering will be applied. Applicable only when the offerring’s product is a termed service |                                                                                                         |