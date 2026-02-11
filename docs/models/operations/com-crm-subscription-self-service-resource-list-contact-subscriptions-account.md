# ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsAccount

The account of the Subscription. Account might be owned by a Contact or an Organisation

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsAccount } from "crm/models/operations";

let value:
  ComCrmSubscriptionSelfServiceResourceListContactSubscriptionsAccount = {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "Universal Name",
    number: "23114132",
    currencyCode: "EUR",
  };
```

## Fields

| Field                                    | Type                                     | Required                                 | Description                              | Example                                  |
| ---------------------------------------- | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
| `id`                                     | *string*                                 | :heavy_minus_sign:                       | The entity identifier                    | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0     |
| `name`                                   | *string*                                 | :heavy_minus_sign:                       | The account name                         | Universal Name                           |
| `number`                                 | *string*                                 | :heavy_minus_sign:                       | The account number                       | 23114132                                 |
| `currencyCode`                           | *string*                                 | :heavy_minus_sign:                       | Currency code based on ISO 4217 standard | EUR                                      |