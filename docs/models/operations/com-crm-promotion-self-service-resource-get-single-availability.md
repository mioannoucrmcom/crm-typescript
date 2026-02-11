# ComCrmPromotionSelfServiceResourceGetSingleAvailability

Determines when the Promotion is available and will be applied. A Promotion is applied only when purchases are performed within this period.

## Example Usage

```typescript
import { ComCrmPromotionSelfServiceResourceGetSingleAvailability } from "crmcom/models/operations";

let value: ComCrmPromotionSelfServiceResourceGetSingleAvailability = {
  fromDate: 1648067185,
  toDate: 1648067185,
};
```

## Fields

| Field                                                                | Type                                                                 | Required                                                             | Description                                                          | Example                                                              |
| -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| `fromDate`                                                           | *number*                                                             | :heavy_minus_sign:                                                   | Contacts get the Promotion on orders performed from this date onward | 1648067185                                                           |
| `toDate`                                                             | *number*                                                             | :heavy_minus_sign:                                                   | Promotion applied on orders up until this date                       | 1648067185                                                           |