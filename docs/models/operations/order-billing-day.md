# OrderBillingDay

## Example Usage

```typescript
import { OrderBillingDay } from "crmcom/models/operations";

let value: OrderBillingDay = {
  dayOfWeek: "MONDAY",
  dayOfMonth: 5,
  monthOfYear: "JANUARY",
};
```

## Fields

| Field              | Type               | Required           | Description        | Example            |
| ------------------ | ------------------ | ------------------ | ------------------ | ------------------ |
| `dayOfWeek`        | *string*           | :heavy_minus_sign: | Day of week        | MONDAY             |
| `dayOfMonth`       | *number*           | :heavy_minus_sign: | Day of month       | 5                  |
| `monthOfYear`      | *string*           | :heavy_minus_sign: | Month of year      | JANUARY            |