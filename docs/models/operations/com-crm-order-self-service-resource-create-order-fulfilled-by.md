# ComCrmOrderSelfServiceResourceCreateOrderFulfilledBy

The organisation that will fulfill the Order

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceCreateOrderFulfilledBy } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourceCreateOrderFulfilledBy = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Bro Burgers",
  phone: "+6934222321",
  address: {
    addressLine1: "Elia Papakyriakou 21",
    addressLine2: "7 Tower Stars",
    stateProvinceCounty: "Egkomi",
    townCity: "Nicosia",
    postalCode: "2415",
    lat: 35.157115,
    lon: 33.313719,
    googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
  },
};
```

## Fields

| Field                                                                                                                                              | Type                                                                                                                                               | Required                                                                                                                                           | Description                                                                                                                                        | Example                                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                               | *string*                                                                                                                                           | :heavy_minus_sign:                                                                                                                                 | The entity identifier                                                                                                                              | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                               |
| `name`                                                                                                                                             | *string*                                                                                                                                           | :heavy_minus_sign:                                                                                                                                 | The name of the organisation                                                                                                                       | Bro Burgers                                                                                                                                        |
| `phone`                                                                                                                                            | *string*                                                                                                                                           | :heavy_minus_sign:                                                                                                                                 | The organisation’s phone number                                                                                                                    | +6934222321                                                                                                                                        |
| `address`                                                                                                                                          | [operations.ComCrmOrderSelfServiceResourceCreateOrderAddress](../../models/operations/com-crm-order-self-service-resource-create-order-address.md) | :heavy_minus_sign:                                                                                                                                 | Information about the organisation’s location                                                                                                      |                                                                                                                                                    |