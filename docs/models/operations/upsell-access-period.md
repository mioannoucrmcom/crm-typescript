# UpsellAccessPeriod

The period of time that service will be accessible. Applicable only for one-time services

## Example Usage

```typescript
import { UpsellAccessPeriod } from "crm/models/operations";

let value: UpsellAccessPeriod = {
  startDate: 1612953199,
  endDate: 1612953199,
};
```

## Fields

| Field                                         | Type                                          | Required                                      | Description                                   | Example                                       |
| --------------------------------------------- | --------------------------------------------- | --------------------------------------------- | --------------------------------------------- | --------------------------------------------- |
| `startDate`                                   | *number*                                      | :heavy_minus_sign:                            | The date that the One Time service will start | 1612953199                                    |
| `endDate`                                     | *number*                                      | :heavy_minus_sign:                            | The date that the One Time service will end   | 1612953199                                    |