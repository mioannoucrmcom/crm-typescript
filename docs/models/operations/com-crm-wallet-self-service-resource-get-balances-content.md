# ComCrmWalletSelfServiceResourceGetBalancesContent

## Example Usage

```typescript
import { ComCrmWalletSelfServiceResourceGetBalancesContent } from "crm/models/operations";

let value: ComCrmWalletSelfServiceResourceGetBalancesContent = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Happy Hour",
  description:
    "Visit Coffee Shop any weekday early afternoon (3 to 5 pm) for happy hour",
  amount: 100.5,
  currencyCode: "EUR",
  expiration: {
    zeroToThirty: 30,
    thirtyToSixty: 50.5,
    sixtyToNinety: 55.5,
    ninetyPlus: 60,
  },
  organisations: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Cafe",
      type: "MERCHANT",
      locations: [
        {
          name: "Head Office",
          addressLine1: "Elia Papakyriakou 21",
          addressLine2: "7 Stars Tower",
          stateProvinceCounty: "Egkomi",
          townCity: "Nicosia",
          postalCode: "2415",
          countryCode: "CYP",
          lat: 35.157115,
          lon: 33.313719,
          googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
        },
      ],
    },
  ],
  products: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Coffee",
      description: "Brazilian Coffee",
      sku: "COF-5541",
    },
  ],
  timings: [
    {
      day: 1,
      month: 10,
      startTime: "19:00",
      endTime: "21:00",
    },
  ],
  applicableForActivation: true,
  isActive: true,
  b2bDetails: {
    isPublished: true,
    isPromoted: true,
    promotedOrganisation: {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Universal Name",
    },
  },
};
```

## Fields

| Field                                                                                                                                                            | Type                                                                                                                                                             | Required                                                                                                                                                         | Description                                                                                                                                                      | Example                                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                             | *string*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | The entity identifier                                                                                                                                            | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                             |
| `name`                                                                                                                                                           | *string*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | The name of the commerce pools group                                                                                                                             | Happy Hour                                                                                                                                                       |
| `description`                                                                                                                                                    | *string*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | The description of the commerce pools group                                                                                                                      | Visit Coffee Shop any weekday early afternoon (3 to 5 pm) for happy hour                                                                                         |
| `amount`                                                                                                                                                         | *number*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | The amount that is allocated to the specified commerce pool                                                                                                      | 100.5                                                                                                                                                            |
| `currencyCode`                                                                                                                                                   | *string*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | Currency code based on ISO 4217 standard                                                                                                                         | EUR                                                                                                                                                              |
| `expiration`                                                                                                                                                     | [operations.Expiration](../../models/operations/expiration.md)                                                                                                   | :heavy_minus_sign:                                                                                                                                               | Defines the amounts expiring in periods. Available only if the parameter include_expiration is set to true                                                       |                                                                                                                                                                  |
| `organisations`                                                                                                                                                  | [operations.ComCrmWalletSelfServiceResourceGetBalancesOrganisation](../../models/operations/com-crm-wallet-self-service-resource-get-balances-organisation.md)[] | :heavy_minus_sign:                                                                                                                                               | The organisations where the amount can be spent at                                                                                                               |                                                                                                                                                                  |
| `products`                                                                                                                                                       | [operations.ComCrmWalletSelfServiceResourceGetBalancesProduct](../../models/operations/com-crm-wallet-self-service-resource-get-balances-product.md)[]           | :heavy_minus_sign:                                                                                                                                               | The products that the amount can be spent for                                                                                                                    |                                                                                                                                                                  |
| `timings`                                                                                                                                                        | [operations.Timing](../../models/operations/timing.md)[]                                                                                                         | :heavy_minus_sign:                                                                                                                                               | The time when the amount can be spent                                                                                                                            |                                                                                                                                                                  |
| `applicableForActivation`                                                                                                                                        | *boolean*                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                               | Indicates if the commerce pool can be activated by the contact                                                                                                   | true                                                                                                                                                             |
| `isActive`                                                                                                                                                       | *boolean*                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                               | Indicates if the commerce pool has been activated                                                                                                                | true                                                                                                                                                             |
| `b2bDetails`                                                                                                                                                     | [operations.B2bDetails](../../models/operations/b2b-details.md)                                                                                                  | :heavy_minus_sign:                                                                                                                                               | Details about commerce pool promote & join information                                                                                                           |                                                                                                                                                                  |