# ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesResponse

OK

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesResponse } from "crmcom/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesResponse = {
    paging: {
      page: 2,
      size: 20,
      total: 5124,
      hasMore: true,
    },
    content: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        state: "EFFECTIVE",
        addedOn: 1625555027,
        firstActivatedOn: 1625555027,
        removedOn: 1625555027,
        isRecurringCharge: true,
        hasAllowance: true,
        scheduledActions: true,
        product: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          classification: "ONE_TIME_SERVICE",
          typeComposition: "FLAT",
          instanceModel: "QUANTITY_BASED",
        },
        price: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          price: 9.99,
          currencyCode: "EUR",
          billingPeriod: {
            duration: 1,
            uot: "MONTH",
          },
        },
        billing: {
          billedFrom: 1625555027,
          billedTo: 1625555027,
        },
        terms: {
          billingModel: "PRE_BILL",
          autoRenew: true,
          inContract: true,
          contractPeriod: {
            uot: "MONTH",
            startDate: 1625555027,
            endDate: 1625555027,
          },
          termedPeriod: {
            billingCycles: 1,
            startDate: 1625555027,
            endDate: 1625555027,
          },
          quantity: 1,
        },
        trialPeriod: {
          startDate: 1625555027,
          endDate: 1625555027,
          duration: 7,
          uot: "DAY",
          trialState: "IN_TRIAL",
        },
        pausedPeriod: {
          startDate: 1625555027,
          endDate: 1625555027,
        },
        bundledService: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          product: {
            id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
            name: "Universal Name",
            sku: "S0001",
          },
        },
        bundledDevice: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          serialNumber: "STB3332222111",
          product: {
            id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
            name: "Universal Name",
            sku: "S0001",
          },
        },
        subscription: {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          code: "60012321123",
          terms: {
            billingPeriod: {
              duration: 1,
              uot: "MONTH",
            },
            billingDay: {
              dayOfWeek: "MONDAY",
              dayOfMonth: 5,
              monthOfYear: "JANUARY",
            },
            paymentMethod: {
              type: "CARD",
              identity: {
                id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
                identifier: "Visa *****1234 03/25",
              },
            },
            billingModel: "PRE_BILL",
          },
        },
        startDate: 1620981309,
        lastActivatedOn: 1620981309,
        lastDeactivatedOn: 1620981309,
        components: [
          {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
            addedOn: 1625555027,
            firstActivatedOn: 1625555027,
            product: {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
            price: {
              price: 9.99,
              currencyCode: "EUR",
            },
            state: "EFFECTIVE",
            inContract: true,
            quantity: 1,
            priceInclusive: true,
            hasAllowance: true,
          },
        ],
        integrations: [
          {
            id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
            name: "Universal Name",
          },
        ],
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                         | Type                                                                                                                                                                                          | Required                                                                                                                                                                                      | Description                                                                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                      | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesPaging](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-paging.md)     | :heavy_minus_sign:                                                                                                                                                                            | N/A                                                                                                                                                                                           |
| `content`                                                                                                                                                                                     | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesContent](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-content.md)[] | :heavy_minus_sign:                                                                                                                                                                            | N/A                                                                                                                                                                                           |