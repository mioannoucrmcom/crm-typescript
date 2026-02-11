# ComCrmPromotionSelfServiceResourceListAvailability

Period of time during which the Promotion is available i.e. the promotion is applied only for purchases performed within this period

## Example Usage

```typescript
import { ComCrmPromotionSelfServiceResourceListAvailability } from "crm/models/operations";

let value: ComCrmPromotionSelfServiceResourceListAvailability = {
  fromDate: 1648067185,
  toDate: 1648067185,
};
```

## Fields

| Field                                                                | Type                                                                 | Required                                                             | Description                                                          | Example                                                              |
| -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| `fromDate`                                                           | *number*                                                             | :heavy_minus_sign:                                                   | Contacts get the Promotion on orders performed from this date onward | 1648067185                                                           |
| `toDate`                                                             | *number*                                                             | :heavy_minus_sign:                                                   | Promotion applied on orders up until this date                       | 1648067185                                                           |