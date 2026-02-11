# ComCrmSubscriptionSelfServiceResourceChangeBillingDay

Required when changing the billing day of the subscription's terms. A subscription's billing day can only be changed in Anniversary billing models

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceChangeBillingDay } from "crm/models/operations";

let value: ComCrmSubscriptionSelfServiceResourceChangeBillingDay = {
  dayOfWeek: "MONDAY",
  dayOfMonth: 1,
};
```

## Fields

| Field              | Type               | Required           | Description        | Example            |
| ------------------ | ------------------ | ------------------ | ------------------ | ------------------ |
| `dayOfWeek`        | *string*           | :heavy_minus_sign: | Day of week        | MONDAY             |
| `dayOfMonth`       | *number*           | :heavy_minus_sign: | Day of month       | 1                  |