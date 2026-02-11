# CrossSellAccessPeriod

The period of time that service will be accessible. Applicable only for one-time services

## Example Usage

```typescript
import { CrossSellAccessPeriod } from "crmcom/models/operations";

let value: CrossSellAccessPeriod = {
  startDate: 1612953199,
  endDate: 1612953199,
};
```

## Fields

| Field                                         | Type                                          | Required                                      | Description                                   | Example                                       |
| --------------------------------------------- | --------------------------------------------- | --------------------------------------------- | --------------------------------------------- | --------------------------------------------- |
| `startDate`                                   | *number*                                      | :heavy_minus_sign:                            | The date that the One Time service will start | 1612953199                                    |
| `endDate`                                     | *number*                                      | :heavy_minus_sign:                            | The date that the One Time service will end   | 1612953199                                    |