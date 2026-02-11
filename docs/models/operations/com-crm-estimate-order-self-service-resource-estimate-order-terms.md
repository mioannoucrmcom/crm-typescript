# ComCrmEstimateOrderSelfServiceResourceEstimateOrderTerms

## Example Usage

```typescript
import { ComCrmEstimateOrderSelfServiceResourceEstimateOrderTerms } from "crmcom/models/operations";

let value: ComCrmEstimateOrderSelfServiceResourceEstimateOrderTerms = {
  billingPeriod: {
    duration: 1,
    uot: "MONTH",
  },
  billingDay: {
    dayOfWeek: "MONDAY",
    dayOfMonth: 5,
    monthOfYear: "JANUARY",
  },
  billingModel: "PRE_BILL",
};
```

## Fields

| Field                                                                                                                                                                                | Type                                                                                                                                                                                 | Required                                                                                                                                                                             | Description                                                                                                                                                                          | Example                                                                                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `billingPeriod`                                                                                                                                                                      | [operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderBillingPeriod](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-billing-period.md) | :heavy_minus_sign:                                                                                                                                                                   | N/A                                                                                                                                                                                  |                                                                                                                                                                                      |
| `billingDay`                                                                                                                                                                         | [operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderBillingDay](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-billing-day.md)       | :heavy_minus_sign:                                                                                                                                                                   | N/A                                                                                                                                                                                  |                                                                                                                                                                                      |
| `billingModel`                                                                                                                                                                       | [operations.ComCrmEstimateOrderSelfServiceResourceEstimateOrderBillingModel](../../models/operations/com-crm-estimate-order-self-service-resource-estimate-order-billing-model.md)   | :heavy_minus_sign:                                                                                                                                                                   | N/A                                                                                                                                                                                  | PRE_BILL                                                                                                                                                                             |