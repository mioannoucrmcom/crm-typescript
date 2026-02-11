# ComCrmPromotionSelfServiceResourceGetSingleContractPeriod

The contract period of the basket item. Applicable only for termed services. The contract period is the one specified in the service’s price terms selected on ordering

## Example Usage

```typescript
import { ComCrmPromotionSelfServiceResourceGetSingleContractPeriod } from "crmcom/models/operations";

let value: ComCrmPromotionSelfServiceResourceGetSingleContractPeriod = {
  duration: 12,
  uot: "MONTH",
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       | Example                                                                                           |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `duration`                                                                                        | *number*                                                                                          | :heavy_minus_sign:                                                                                | Contract period duration                                                                          | 12                                                                                                |
| `uot`                                                                                             | [operations.ConditionContractPeriodUot](../../models/operations/condition-contract-period-uot.md) | :heavy_minus_sign:                                                                                | Contract period unit of time                                                                      | MONTH                                                                                             |