# ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceServiceResponse

## Example Usage

```typescript
import { ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceServiceResponse } from "crm/models/operations";

let value:
  ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceServiceResponse =
    {
      authoriseConsumption: true,
      currencyCode: "EUR",
      service: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        classification: "TRACEABLE_PHYSICAL_GOOD",
        product: {
          id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
          name: "Universal Name",
          sku: "S0001",
        },
      },
      accumulatedAllowance: {
        cashAmounts: {
          perTransaction: 59.99,
          perDay: 19.99,
          perBillingCycle: 9.99,
        },
      },
      productsAllowance: [
        {
          itemType: "PRODUCT",
          remainingCash: {
            perTransaction: 59.99,
            perDay: 19.99,
            perBillingCycle: 9.99,
          },
          remainingUsage: {
            perTransaction: 59.99,
            perDay: 19.99,
            perBillingCycle: 9.99,
          },
          measurementUnit: {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          },
        },
      ],
    };
```

## Fields

| Field                                                                                                                                                                                                                     | Type                                                                                                                                                                                                                      | Required                                                                                                                                                                                                                  | Description                                                                                                                                                                                                               | Example                                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `authoriseConsumption`                                                                                                                                                                                                    | *boolean*                                                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                                                        | Returned as True if usage can be consumed, i.e. termed/one-time service has remaining allowance. If no usage allowance limits are set, then usage is always authorised.                                                   | true                                                                                                                                                                                                                      |
| `currencyCode`                                                                                                                                                                                                            | [operations.ServiceCurrencyCode](../../models/operations/service-currency-code.md)                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                        | The currency code used in usage allowance cash amount limits                                                                                                                                                              | EUR                                                                                                                                                                                                                       |
| `service`                                                                                                                                                                                                                 | [operations.ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceServiceServiceResponse](../../models/operations/com-crm-estimate-allowance-self-service-resource-estimates-allowance-service-service-response.md) | :heavy_minus_sign:                                                                                                                                                                                                        | The one-time/termed service through which usage is consumed                                                                                                                                                               |                                                                                                                                                                                                                           |
| `accumulatedAllowance`                                                                                                                                                                                                    | [operations.ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceAccumulatedAllowance](../../models/operations/com-crm-estimate-allowance-self-service-resource-estimates-allowance-accumulated-allowance.md)      | :heavy_minus_sign:                                                                                                                                                                                                        | N/A                                                                                                                                                                                                                       |                                                                                                                                                                                                                           |
| `productsAllowance`                                                                                                                                                                                                       | [operations.ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceProductsAllowance](../../models/operations/com-crm-estimate-allowance-self-service-resource-estimates-allowance-products-allowance.md)[]          | :heavy_minus_sign:                                                                                                                                                                                                        | N/A                                                                                                                                                                                                                       |                                                                                                                                                                                                                           |