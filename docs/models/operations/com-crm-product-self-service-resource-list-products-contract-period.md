# ComCrmProductSelfServiceResourceListProductsContractPeriod

The service's contract period (if any)

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceListProductsContractPeriod } from "crmcom/models/operations";

let value: ComCrmProductSelfServiceResourceListProductsContractPeriod = {
  duration: 2,
  uot: "MINUTE",
};
```

## Fields

| Field                                                                                                                                                                          | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    | Example                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `duration`                                                                                                                                                                     | *number*                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                             | Period Cycle duration                                                                                                                                                          | 2                                                                                                                                                                              |
| `uot`                                                                                                                                                                          | [operations.ComCrmProductSelfServiceResourceListProductsContractPeriodUot](../../models/operations/com-crm-product-self-service-resource-list-products-contract-period-uot.md) | :heavy_minus_sign:                                                                                                                                                             | Period Cycle unit of time                                                                                                                                                      | MONTHS                                                                                                                                                                         |