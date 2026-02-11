# ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesContent

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesContent } from "crm/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesContent = {
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
  };
```

## Fields

| Field                                                                                                                                                                                                  | Type                                                                                                                                                                                                   | Required                                                                                                                                                                                               | Description                                                                                                                                                                                            | Example                                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                                                   | *string*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | The entity identifier                                                                                                                                                                                  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                   |
| `state`                                                                                                                                                                                                | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesState](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-state.md)                | :heavy_minus_sign:                                                                                                                                                                                     | Subscription Service's State                                                                                                                                                                           | EFFECTIVE                                                                                                                                                                                              |
| `addedOn`                                                                                                                                                                                              | *number*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | Date added to the subscription                                                                                                                                                                         | 1625555027                                                                                                                                                                                             |
| `firstActivatedOn`                                                                                                                                                                                     | *number*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | First activation date                                                                                                                                                                                  | 1625555027                                                                                                                                                                                             |
| `removedOn`                                                                                                                                                                                            | *number*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | Date removed from the subscription (applies for churned services)                                                                                                                                      | 1625555027                                                                                                                                                                                             |
| `isRecurringCharge`                                                                                                                                                                                    | *boolean*                                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                     | Applicable for expense services to indicate whether they are charged on a recurring basis                                                                                                              | true                                                                                                                                                                                                   |
| `hasAllowance`                                                                                                                                                                                         | *boolean*                                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                     | Shows whether the service allows subscribers to consume usage                                                                                                                                          | true                                                                                                                                                                                                   |
| `scheduledActions`                                                                                                                                                                                     | *boolean*                                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                     | Shows whether there are pending scheduled actions for the service                                                                                                                                      | true                                                                                                                                                                                                   |
| `product`                                                                                                                                                                                              | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesProduct](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-product.md)            | :heavy_minus_sign:                                                                                                                                                                                     | Service product information                                                                                                                                                                            |                                                                                                                                                                                                        |
| `price`                                                                                                                                                                                                | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesPrice](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-price.md)                | :heavy_minus_sign:                                                                                                                                                                                     | Service pricing information                                                                                                                                                                            |                                                                                                                                                                                                        |
| `billing`                                                                                                                                                                                              | [operations.Billing](../../models/operations/billing.md)                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | Latest billing information of the service                                                                                                                                                              |                                                                                                                                                                                                        |
| `terms`                                                                                                                                                                                                | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesTerms](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-terms.md)                | :heavy_minus_sign:                                                                                                                                                                                     | Services's price terms                                                                                                                                                                                 |                                                                                                                                                                                                        |
| `trialPeriod`                                                                                                                                                                                          | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesTrialPeriod](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-trial-period.md)   | :heavy_minus_sign:                                                                                                                                                                                     | Service's trial period details                                                                                                                                                                         |                                                                                                                                                                                                        |
| `pausedPeriod`                                                                                                                                                                                         | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesPausedPeriod](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-paused-period.md) | :heavy_minus_sign:                                                                                                                                                                                     | Applicable while the service is paused                                                                                                                                                                 |                                                                                                                                                                                                        |
| `bundledService`                                                                                                                                                                                       | [operations.BundledService](../../models/operations/bundled-service.md)                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                                     | Applicable when the service was added as part of a bundled service                                                                                                                                     |                                                                                                                                                                                                        |
| `bundledDevice`                                                                                                                                                                                        | [operations.BundledDevice](../../models/operations/bundled-device.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                                     | Applicable when the service was added as part of a bundled device                                                                                                                                      |                                                                                                                                                                                                        |
| `subscription`                                                                                                                                                                                         | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesSubscription](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-subscription.md)  | :heavy_minus_sign:                                                                                                                                                                                     | The subscription of the service                                                                                                                                                                        |                                                                                                                                                                                                        |
| `startDate`                                                                                                                                                                                            | *number*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | The date on which the service is scheduled to be added on the subscription                                                                                                                             | 1620981309                                                                                                                                                                                             |
| `order`                                                                                                                                                                                                | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesContentOrder](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-content-order.md) | :heavy_minus_sign:                                                                                                                                                                                     | The order related to the service                                                                                                                                                                       |                                                                                                                                                                                                        |
| `lastActivatedOn`                                                                                                                                                                                      | *number*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | Τhe most recent date on which the service was activated                                                                                                                                                | 1620981309                                                                                                                                                                                             |
| `lastDeactivatedOn`                                                                                                                                                                                    | *number*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | Τhe most recent date on which the service was deactivated (via a Deactivate service action that changed the service’s state to Not Effective)                                                          | 1620981309                                                                                                                                                                                             |
| `components`                                                                                                                                                                                           | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesComponent](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-component.md)[]      | :heavy_minus_sign:                                                                                                                                                                                     | Applicable for bundle services and returns a list of component services                                                                                                                                |                                                                                                                                                                                                        |
| `integrations`                                                                                                                                                                                         | [operations.ComCrmSubscriptionSelfServiceResourceListSubscriptionServicesIntegration](../../models/operations/com-crm-subscription-self-service-resource-list-subscription-services-integration.md)[]  | :heavy_minus_sign:                                                                                                                                                                                     | The integrations related to the service                                                                                                                                                                |                                                                                                                                                                                                        |