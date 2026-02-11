# ComCrmContactSelfServiceResourceListContactRelationshipUsageAllowance

Defines the usage allowance

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceListContactRelationshipUsageAllowance } from "crm/models/operations";

let value:
  ComCrmContactSelfServiceResourceListContactRelationshipUsageAllowance = {
    accumulatedAllowance: {
      currency: "EUR",
    },
    productsAllowance: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        currency: "EUR",
        itemType: "PRODUCT",
        itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
        name: "Bronze",
        measurementUnit: {
          name: "Gigabytes",
          displayName: "GB",
        },
      },
    ],
    organisations: [
      {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                                                                                           | Type                                                                                                                                                                                                                                                            | Required                                                                                                                                                                                                                                                        | Description                                                                                                                                                                                                                                                     |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `accumulatedAllowance`                                                                                                                                                                                                                                          | [operations.ComCrmContactSelfServiceResourceListContactRelationshipAccumulatedAllowance](../../models/operations/com-crm-contact-self-service-resource-list-contact-relationship-accumulated-allowance.md)                                                      | :heavy_minus_sign:                                                                                                                                                                                                                                              | The community's accumulated cash allowance, i.e. how much can be consumed among all products which are consumed through the community. This allowance is defined only in amount of money and it's evaluated based on the usage's rating (how much it costs)     |
| `sameAsOwner`                                                                                                                                                                                                                                                   | *boolean*                                                                                                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                                                                                              | If set to true, the member has the same usage allowance per product as the owner’s termed/one-time service.                                                                                                                                                     |
| `productsAllowance`                                                                                                                                                                                                                                             | [operations.ComCrmContactSelfServiceResourceListContactRelationshipProductsAllowance](../../models/operations/com-crm-contact-self-service-resource-list-contact-relationship-products-allowance.md)[]                                                          | :heavy_minus_sign:                                                                                                                                                                                                                                              | List of items which can be consumed through the community. This set of items includes usage and non-traceable physical goods. If nothing is specified, then usage is allowed among all usage services/non-traceable physical goods that the business is selling |
| `organisations`                                                                                                                                                                                                                                                 | [operations.ComCrmContactSelfServiceResourceListContactRelationshipOrganisation](../../models/operations/com-crm-contact-self-service-resource-list-contact-relationship-organisation.md)[]                                                                     | :heavy_minus_sign:                                                                                                                                                                                                                                              | The allowed organisations to consume allowance                                                                                                                                                                                                                  |