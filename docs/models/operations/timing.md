# Timing

## Example Usage

```typescript
import { Timing } from "crm/models/operations";

let value: Timing = {
  day: 1,
  month: 10,
  startTime: "19:00",
  endTime: "21:00",
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         | Example                                             |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `day`                                               | *number*                                            | :heavy_minus_sign:                                  | The day of the week as condition (1-7), 1 is Sunday | 1                                                   |
| `month`                                             | *number*                                            | :heavy_minus_sign:                                  | The month as a condition (1-12), 1 is January       | 10                                                  |
| `startTime`                                         | *string*                                            | :heavy_minus_sign:                                  | The start time of the day in 24 Hour format         | 19:00                                               |
| `endTime`                                           | *string*                                            | :heavy_minus_sign:                                  | The end time of the day in 24 Hour format           | 21:00                                               |