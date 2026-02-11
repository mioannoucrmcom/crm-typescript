# ComCrmOrderSelfServiceResourceCreateOrderResponse

Created

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceCreateOrderResponse } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourceCreateOrderResponse = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  number: "O000001",
  fulfilledBy: {
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
  },
  estimatedDeliveryTime: {
    timeToDelivery: 20,
    uot: "MINUTE",
    deliveryAt: 1599224678,
  },
};
```

## Fields

| Field                                                                                                                                                       | Type                                                                                                                                                        | Required                                                                                                                                                    | Description                                                                                                                                                 | Example                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                        | *string*                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                          | The entity identifier                                                                                                                                       | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                        |
| `number`                                                                                                                                                    | *string*                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                          | The Order’s number                                                                                                                                          | O000001                                                                                                                                                     |
| `fulfilledBy`                                                                                                                                               | [operations.ComCrmOrderSelfServiceResourceCreateOrderFulfilledBy](../../models/operations/com-crm-order-self-service-resource-create-order-fulfilled-by.md) | :heavy_minus_sign:                                                                                                                                          | The organisation that will fulfill the Order                                                                                                                |                                                                                                                                                             |
| `estimatedDeliveryTime`                                                                                                                                     | [operations.EstimatedDeliveryTime](../../models/operations/estimated-delivery-time.md)                                                                      | :heavy_minus_sign:                                                                                                                                          | An estimation of the delivery time                                                                                                                          |                                                                                                                                                             |