# ComCrmOrderSelfServiceResourceGetOrderFulfilledBy

Details about the organisation from where such event was posted

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceGetOrderFulfilledBy } from "crm/models/operations";

let value: ComCrmOrderSelfServiceResourceGetOrderFulfilledBy = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "CRM Nicosia",
  phone: "+6934222321",
  address: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    addressLine1: "Elia Papakyriakou 21",
    addressLine2: "7 Tower Stars",
    stateProvinceCounty: "Egkomi",
    townCity: "Nicosia",
    postalCode: "2415",
    countryCode: "CYP",
    lat: 35.157115,
    lon: 33.313719,
    googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
  },
};
```

## Fields

| Field                                                                                                                                                                | Type                                                                                                                                                                 | Required                                                                                                                                                             | Description                                                                                                                                                          | Example                                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                 | *string*                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                   | The entity identifier                                                                                                                                                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                 |
| `name`                                                                                                                                                               | *string*                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                   | The name of the organisation                                                                                                                                         | CRM Nicosia                                                                                                                                                          |
| `phone`                                                                                                                                                              | *string*                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                   | The organisation’s phone number                                                                                                                                      | +6934222321                                                                                                                                                          |
| `address`                                                                                                                                                            | [operations.ComCrmOrderSelfServiceResourceGetOrderFulfilledByAddress](../../models/operations/com-crm-order-self-service-resource-get-order-fulfilled-by-address.md) | :heavy_minus_sign:                                                                                                                                                   | Information about the organisation’s location                                                                                                                        |                                                                                                                                                                      |