# BillingCycle

The billing cycle of the basket item. Applicable only for termed services. The billing cycle is the one specified in the service’s price terms selected on ordering

## Example Usage

```typescript
import { BillingCycle } from "crm/models/operations";

let value: BillingCycle = {
  duration: 1,
  uot: "DAY",
};
```

## Fields

| Field                                                                      | Type                                                                       | Required                                                                   | Description                                                                | Example                                                                    |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| `duration`                                                                 | *number*                                                                   | :heavy_check_mark:                                                         | Billing cycle duration                                                     | 1                                                                          |
| `uot`                                                                      | [operations.BillingCycleUot](../../models/operations/billing-cycle-uot.md) | :heavy_check_mark:                                                         | Billing cycle unit of time                                                 | DAY                                                                        |