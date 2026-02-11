# TimingsAvailability

## Example Usage

```typescript
import { TimingsAvailability } from "crm/models/operations";

let value: TimingsAvailability = {
  day: 1,
  month: 1,
  startTime: "13:00",
  endTime: "14:00",
};
```

## Fields

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          | Example                                                                              |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `day`                                                                                | *number*                                                                             | :heavy_minus_sign:                                                                   | Day of week. Allowed values are 1 to 7, where 1 is Sunday                            | 1                                                                                    |
| `month`                                                                              | *number*                                                                             | :heavy_minus_sign:                                                                   | Month during which promotion is applied. Allowed values are 1-12, where 1 is January | 1                                                                                    |
| `startTime`                                                                          | *string*                                                                             | :heavy_minus_sign:                                                                   | Starting time                                                                        | 13:00                                                                                |
| `endTime`                                                                            | *string*                                                                             | :heavy_minus_sign:                                                                   | End time                                                                             | 14:00                                                                                |