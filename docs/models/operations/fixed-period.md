# FixedPeriod

Promotion is applied if the purchase is performed within the specified period of time. Either a fixed period or promotion availability must be specified

## Example Usage

```typescript
import { FixedPeriod } from "crm/models/operations";

let value: FixedPeriod = {
  startDate: 1648067185,
  endDate: 1648067185,
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       | Example                                                                           |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `startDate`                                                                       | *number*                                                                          | :heavy_check_mark:                                                                | Promotion applied if purchase is performed from this date (inclusive) and onwards | 1648067185                                                                        |
| `endDate`                                                                         | *number*                                                                          | :heavy_minus_sign:                                                                | If specified, then the purchase must be performed up until this date (Optional)   | 1648067185                                                                        |