# Timings

Promotion timings

## Example Usage

```typescript
import { Timings } from "crmcom/models/operations";

let value: Timings = {
  fixedPeriod: {
    startDate: 1648067185,
    endDate: 1648067185,
  },
  availability: [
    {
      day: 1,
      month: 1,
      startTime: "13:00",
      endTime: "14:00",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                                              | Type                                                                                                                                                                                                               | Required                                                                                                                                                                                                           | Description                                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `fixedPeriod`                                                                                                                                                                                                      | [operations.FixedPeriod](../../models/operations/fixed-period.md)                                                                                                                                                  | :heavy_check_mark:                                                                                                                                                                                                 | Promotion is applied if the purchase is performed within the specified period of time. Either a fixed period or promotion availability must be specified                                                           |
| `availability`                                                                                                                                                                                                     | [operations.TimingsAvailability](../../models/operations/timings-availability.md)[]                                                                                                                                | :heavy_check_mark:                                                                                                                                                                                                 | Promotion is applied if the purchase is performed within the specified day(s), month(s) and/or times. Either a fixed period or promotion availability must be specified. Each availibility option should be unique |