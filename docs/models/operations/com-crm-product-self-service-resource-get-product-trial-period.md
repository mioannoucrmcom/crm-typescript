# ComCrmProductSelfServiceResourceGetProductTrialPeriod

Shows if the service will get a trial period

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductTrialPeriod } from "crmcom/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductTrialPeriod = {
  duration: 2,
  uot: "DAY",
};
```

## Fields

| Field                                                                                                                                                                | Type                                                                                                                                                                 | Required                                                                                                                                                             | Description                                                                                                                                                          | Example                                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `duration`                                                                                                                                                           | *number*                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                   | Period Cycle duration                                                                                                                                                | 2                                                                                                                                                                    |
| `uot`                                                                                                                                                                | [operations.ComCrmProductSelfServiceResourceGetProductTrialPeriodUot](../../models/operations/com-crm-product-self-service-resource-get-product-trial-period-uot.md) | :heavy_minus_sign:                                                                                                                                                   | Period Cycle unit of time                                                                                                                                            | MONTHS                                                                                                                                                               |