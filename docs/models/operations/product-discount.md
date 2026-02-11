# ProductDiscount

The discount provided to the ordered item

## Example Usage

```typescript
import { ProductDiscount } from "crm/models/operations";

let value: ProductDiscount = {};
```

## Fields

| Field                                       | Type                                        | Required                                    | Description                                 |
| ------------------------------------------- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------- |
| `amount`                                    | *number*                                    | :heavy_minus_sign:                          | The applied discount amount excluding taxes |
| `amountInclTax`                             | *number*                                    | :heavy_minus_sign:                          | The applied disocunt with its taxed amount  |
| `percentage`                                | *number*                                    | :heavy_minus_sign:                          | The applied discount percentage             |