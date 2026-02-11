# ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceResponse

OK

## Example Usage

```typescript
import { ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceResponse } from "crmcom/models/operations";

let value:
  ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceResponse = {
    estimationId: "784efd68-3d22-3682-fd86-f28fe270dbe3",
    services: [
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
      },
    ],
    authorisedUsage: [
      {
        product: {
          id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
          name: "Universal Name",
          sku: "S0001",
        },
        measurementUnit: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        },
        services: [
          {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
            classification: "TRACEABLE_PHYSICAL_GOOD",
            product: {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
          },
        ],
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                                                                                                                                                                                                                                                        | Type                                                                                                                                                                                                                                                                                                                                                                                                                         | Required                                                                                                                                                                                                                                                                                                                                                                                                                     | Description                                                                                                                                                                                                                                                                                                                                                                                                                  | Example                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `estimationId`                                                                                                                                                                                                                                                                                                                                                                                                               | *string*                                                                                                                                                                                                                                                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                                                                                           | Includes detailed information of the requested and authorised usage to be consumed. Can be used in a sub-sequent call to add a new usage record with the same usage information                                                                                                                                                                                                                                              | 784efd68-3d22-3682-fd86-f28fe270dbe3                                                                                                                                                                                                                                                                                                                                                                                         |
| `services`                                                                                                                                                                                                                                                                                                                                                                                                                   | [operations.ComCrmEstimateAllowanceSelfServiceResourceEstimatesAllowanceServiceResponse](../../models/operations/com-crm-estimate-allowance-self-service-resource-estimates-allowance-service-response.md)[]                                                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                                                                                           | List of subscription services that allow the contact to consume usage along with the services' allowed and remaining usage                                                                                                                                                                                                                                                                                                   |                                                                                                                                                                                                                                                                                                                                                                                                                              |
| `authorisedUsage`                                                                                                                                                                                                                                                                                                                                                                                                            | [operations.AuthorisedUsage](../../models/operations/authorised-usage.md)[]                                                                                                                                                                                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                                                                                                                                                                                                                                                           | A set of products that have remaining usage allowance. The set includes usage services and non-traceable physical goods. This list includes only the products that still have remaining allowance, across all subscription services. This means that if the same usage products is granded some allowance from more than one services, then the total remaining allowance among all services is returned in a single object. |                                                                                                                                                                                                                                                                                                                                                                                                                              |