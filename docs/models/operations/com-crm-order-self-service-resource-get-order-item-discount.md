# ComCrmOrderSelfServiceResourceGetOrderItemDiscount

Applied discounton the ordered item

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceGetOrderItemDiscount } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourceGetOrderItemDiscount = {};
```

## Fields

| Field                                       | Type                                        | Required                                    | Description                                 |
| ------------------------------------------- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------- |
| `amount`                                    | *number*                                    | :heavy_minus_sign:                          | The applied discount amount excluding taxes |
| `amountInclTax`                             | *number*                                    | :heavy_minus_sign:                          | The applied disocunt with its taxed amount  |
| `percentage`                                | *number*                                    | :heavy_minus_sign:                          | The applied discount percentage             |