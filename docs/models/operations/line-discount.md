# LineDiscount

The applied discount. If a percentage was applied, then retrieving the line's discount will return both the discount amount and the percentage

## Example Usage

```typescript
import { LineDiscount } from "crm/models/operations";

let value: LineDiscount = {
  amount: 20.5,
  percentage: 10,
  amountInclTax: 15.5,
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       | Example                                                                                           |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `amount`                                                                                          | *number*                                                                                          | :heavy_minus_sign:                                                                                | The discount amount of the line. This is the discount excluding the taxed amount for the disocunt | 20.5                                                                                              |
| `percentage`                                                                                      | *number*                                                                                          | :heavy_minus_sign:                                                                                | The discount percentage of the line                                                               | 10                                                                                                |
| `amountInclTax`                                                                                   | *number*                                                                                          | :heavy_minus_sign:                                                                                | The discount amount including applied taxes                                                       | 15.5                                                                                              |