# PeriodSettings

Applicable only for Scheduled actions that include period settings such as Paused period

## Example Usage

```typescript
import { PeriodSettings } from "crm/models/operations";

let value: PeriodSettings = {};
```

## Fields

| Field                             | Type                              | Required                          | Description                       |
| --------------------------------- | --------------------------------- | --------------------------------- | --------------------------------- |
| `durationInDays`                  | *number*                          | :heavy_minus_sign:                | The new period's duration in days |
| `endsOn`                          | *number*                          | :heavy_minus_sign:                | TThe new period's end date        |