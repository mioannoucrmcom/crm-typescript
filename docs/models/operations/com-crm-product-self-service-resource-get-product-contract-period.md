# ComCrmProductSelfServiceResourceGetProductContractPeriod

The service's contract period (if any)

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductContractPeriod } from "crmcom/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductContractPeriod = {
  duration: 2,
  uot: "SECOND",
};
```

## Fields

| Field                                                                                                                                                                      | Type                                                                                                                                                                       | Required                                                                                                                                                                   | Description                                                                                                                                                                | Example                                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `duration`                                                                                                                                                                 | *number*                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                         | Period Cycle duration                                                                                                                                                      | 2                                                                                                                                                                          |
| `uot`                                                                                                                                                                      | [operations.ComCrmProductSelfServiceResourceGetProductContractPeriodUot](../../models/operations/com-crm-product-self-service-resource-get-product-contract-period-uot.md) | :heavy_minus_sign:                                                                                                                                                         | Period Cycle unit of time                                                                                                                                                  | MONTHS                                                                                                                                                                     |