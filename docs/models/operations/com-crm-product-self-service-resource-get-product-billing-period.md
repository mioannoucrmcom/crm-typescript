# ComCrmProductSelfServiceResourceGetProductBillingPeriod

The service's billing cycle

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductBillingPeriod } from "crmcom/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductBillingPeriod = {
  duration: 2,
  uot: "MINUTE",
};
```

## Fields

| Field                                                                                                                                                                    | Type                                                                                                                                                                     | Required                                                                                                                                                                 | Description                                                                                                                                                              | Example                                                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `duration`                                                                                                                                                               | *number*                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                       | Period Cycle duration                                                                                                                                                    | 2                                                                                                                                                                        |
| `uot`                                                                                                                                                                    | [operations.ComCrmProductSelfServiceResourceGetProductBillingPeriodUot](../../models/operations/com-crm-product-self-service-resource-get-product-billing-period-uot.md) | :heavy_minus_sign:                                                                                                                                                       | Period Cycle unit of time                                                                                                                                                | MONTHS                                                                                                                                                                   |