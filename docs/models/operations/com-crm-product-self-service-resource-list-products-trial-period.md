# ComCrmProductSelfServiceResourceListProductsTrialPeriod

Shows if the service will get a trial period

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceListProductsTrialPeriod } from "crmcom/models/operations";

let value: ComCrmProductSelfServiceResourceListProductsTrialPeriod = {
  duration: 2,
  uot: "SECOND",
};
```

## Fields

| Field                                                                                                                                                                    | Type                                                                                                                                                                     | Required                                                                                                                                                                 | Description                                                                                                                                                              | Example                                                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `duration`                                                                                                                                                               | *number*                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                       | Period Cycle duration                                                                                                                                                    | 2                                                                                                                                                                        |
| `uot`                                                                                                                                                                    | [operations.ComCrmProductSelfServiceResourceListProductsTrialPeriodUot](../../models/operations/com-crm-product-self-service-resource-list-products-trial-period-uot.md) | :heavy_minus_sign:                                                                                                                                                       | Period Cycle unit of time                                                                                                                                                | MONTHS                                                                                                                                                                   |