# OrderLineItemPeriod

Termed service’s debited/credited period

## Example Usage

```typescript
import { OrderLineItemPeriod } from "crm/models/operations";

let value: OrderLineItemPeriod = {};
```

## Fields

| Field                                                 | Type                                                  | Required                                              | Description                                           |
| ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- |
| `from`                                                | *number*                                              | :heavy_minus_sign:                                    | The date from which the service is invoiced/credited  |
| `to`                                                  | *number*                                              | :heavy_minus_sign:                                    | The date until which the service is invoiced/credited |