# ComCrmProductSelfServiceResourceListProductsBillingPeriod

The service's billing cycle

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceListProductsBillingPeriod } from "crm/models/operations";

let value: ComCrmProductSelfServiceResourceListProductsBillingPeriod = {
  duration: 2,
  uot: "HOUR",
};
```

## Fields

| Field                                                                                                                                                                        | Type                                                                                                                                                                         | Required                                                                                                                                                                     | Description                                                                                                                                                                  | Example                                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `duration`                                                                                                                                                                   | *number*                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                           | Period Cycle duration                                                                                                                                                        | 2                                                                                                                                                                            |
| `uot`                                                                                                                                                                        | [operations.ComCrmProductSelfServiceResourceListProductsBillingPeriodUot](../../models/operations/com-crm-product-self-service-resource-list-products-billing-period-uot.md) | :heavy_minus_sign:                                                                                                                                                           | Period Cycle unit of time                                                                                                                                                    | MONTHS                                                                                                                                                                       |