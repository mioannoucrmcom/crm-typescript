# TermedPeriod

Service's termed period

## Example Usage

```typescript
import { TermedPeriod } from "crm/models/operations";

let value: TermedPeriod = {
  billingCycles: 1,
  startDate: 1625555027,
  endDate: 1625555027,
};
```

## Fields

| Field                                             | Type                                              | Required                                          | Description                                       | Example                                           |
| ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- |
| `billingCycles`                                   | *number*                                          | :heavy_minus_sign:                                | How many billing cycles each termed period covers | 1                                                 |
| `startDate`                                       | *number*                                          | :heavy_minus_sign:                                | Latest termed period start date                   | 1625555027                                        |
| `endDate`                                         | *number*                                          | :heavy_minus_sign:                                | Termed period end date                            | 1625555027                                        |