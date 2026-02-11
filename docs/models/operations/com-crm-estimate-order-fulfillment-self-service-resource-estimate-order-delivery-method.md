# ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderDeliveryMethod

## Example Usage

```typescript
import { ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderDeliveryMethod } from "crmcom/models/operations";

let value:
  ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderDeliveryMethod =
    {
      type: "PICKUP_POINT",
      deliveryServiceProviders: [
        {
          id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
          name: "ACS",
          creatives: [
            {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              width: 2159,
              height: 3075,
              format: "jpg",
              url: "https://assets.crm.com/image/offer.jpg",
              publicId: "crm-com/image",
              media: [
                {
                  width: 200,
                  height: 300,
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
                },
              ],
            },
          ],
        },
      ],
    };
```

## Fields

| Field                                                                                                                                                                                                                                                                                             | Type                                                                                                                                                                                                                                                                                              | Required                                                                                                                                                                                                                                                                                          | Description                                                                                                                                                                                                                                                                                       | Example                                                                                                                                                                                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                                                                                                                                                                                                                                                                                            | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderType](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-type.md)                                                                                                          | :heavy_minus_sign:                                                                                                                                                                                                                                                                                | The order's delivery method type.                                                                                                                                                                                                                                                                 | DELIVERY                                                                                                                                                                                                                                                                                          |
| `deliveryServiceProviders`                                                                                                                                                                                                                                                                        | [operations.DeliveryServiceProvider](../../models/operations/delivery-service-provider.md)[]                                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                                                                                                                                | The delivery service providers ids. Applicable and required only for COURIER_SERVICE and PICKUP_POINT delivery methods.                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                   |
| `deliveryTimeSelection`                                                                                                                                                                                                                                                                           | [operations.DeliveryTimeSelection](../../models/operations/delivery-time-selection.md)                                                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                                                                                                                                | Defines how the contact selects the delivery time for their order: explicit_delivery_time allows the contact to choose a specific date and time, slot_selection allows them to select from available time slots, and no_time means the delivery date and time are determined by the organisation. |                                                                                                                                                                                                                                                                                                   |