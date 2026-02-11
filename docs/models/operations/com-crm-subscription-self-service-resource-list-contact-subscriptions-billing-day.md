# ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsBillingDay

The day of month/week until which the subscripton's services will be billed. Either a day of month or day of week is returned, depnding on the subscription's billing cycle (if it is less than a month, then a day of week is returned)

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsBillingDay } from "crm/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsBillingDay = {
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