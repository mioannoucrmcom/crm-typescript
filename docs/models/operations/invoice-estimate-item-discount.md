# InvoiceEstimateItemDiscount

## Example Usage

```typescript
import { InvoiceEstimateItemDiscount } from "crm/models/operations";

let value: InvoiceEstimateItemDiscount = {
  discountAmount: 20.5,
  discountPercentage: 10,
};
```

## Fields

| Field                               | Type                                | Required                            | Description                         | Example                             |
| ----------------------------------- | ----------------------------------- | ----------------------------------- | ----------------------------------- | ----------------------------------- |
| `discountAmount`                    | *number*                            | :heavy_minus_sign:                  | The discount amount of the line     | 20.5                                |
| `discountPercentage`                | *number*                            | :heavy_minus_sign:                  | The discount percentage of the line | 10                                  |
| `discountInclTax`                   | *number*                            | :heavy_minus_sign:                  | N/A                                 |                                     |