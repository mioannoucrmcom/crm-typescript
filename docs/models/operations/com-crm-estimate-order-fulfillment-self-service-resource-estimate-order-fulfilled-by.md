# ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderFulfilledBy

## Example Usage

```typescript
import { ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderFulfilledBy } from "crm/models/operations";

let value:
  ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderFulfilledBy = {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "Best Burger Egkomi",
    phone: "+6934222321",
    address: {
      addressLine1: "Ilia Papakyriakou 21",
      addressLine2: "7 Stars Tower",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "2415",
      lat: 35.157115,
      lon: 33.313719,
      googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
    },
    parentOrganisation: {
      id: "b1607c37-e750-2324-ac49-6591a86f54b8",
      name: "Best Burger",
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
              url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
            },
          ],
        },
      ],
    },
    estimatedDelivery: {
      uot: "MINUTE",
    },
    openingHours: [
      {
        dayOfWeek: "MONDAY",
        open: "09:00",
        close: "17:00",
        operation: "DELIVERY",
      },
    ],
    shortTermOperations: [
      {
        isClosed: false,
      },
    ],
    paymentMethodTypes: [
      "CASH",
      "CARD",
    ],
    deliveryMethods: [
      {
        type: "COURIER_SERVICE",
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
      },
    ],
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
            url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
          },
        ],
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                                                    | Type                                                                                                                                                                                                                     | Required                                                                                                                                                                                                                 | Description                                                                                                                                                                                                              | Example                                                                                                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                                                                     | *string*                                                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                                                       | The entity identifier                                                                                                                                                                                                    | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                                     |
| `name`                                                                                                                                                                                                                   | *string*                                                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                                                       | The organisation name                                                                                                                                                                                                    | Best Burger Egkomi                                                                                                                                                                                                       |
| `phone`                                                                                                                                                                                                                  | *string*                                                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                                                       | The organisation phone number                                                                                                                                                                                            | +6934222321                                                                                                                                                                                                              |
| `address`                                                                                                                                                                                                                | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderAddress](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-address.md)                           | :heavy_minus_sign:                                                                                                                                                                                                       | The organisation address                                                                                                                                                                                                 |                                                                                                                                                                                                                          |
| `parentOrganisation`                                                                                                                                                                                                     | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderParentOrganisation](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-parent-organisation.md)    | :heavy_minus_sign:                                                                                                                                                                                                       | Details about the parent organisation (business/merchant) of the fulfilled by. Not applicable if the fulfilled by organisation is of type business or merchant                                                           |                                                                                                                                                                                                                          |
| `estimatedDelivery`                                                                                                                                                                                                      | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderEstimatedDelivery](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-estimated-delivery.md)      | :heavy_minus_sign:                                                                                                                                                                                                       | N/A                                                                                                                                                                                                                      |                                                                                                                                                                                                                          |
| `openingHours`                                                                                                                                                                                                           | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderOpeningHour](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-opening-hour.md)[]                | :heavy_minus_sign:                                                                                                                                                                                                       | Details about the organisation’s working hours                                                                                                                                                                           |                                                                                                                                                                                                                          |
| `shortTermOperations`                                                                                                                                                                                                    | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderShortTermOperation](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-short-term-operation.md)[] | :heavy_minus_sign:                                                                                                                                                                                                       | Details about the organisation’s availability to offer its services                                                                                                                                                      |                                                                                                                                                                                                                          |
| `paymentMethodTypes`                                                                                                                                                                                                     | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderPaymentMethodType](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-payment-method-type.md)[]   | :heavy_minus_sign:                                                                                                                                                                                                       | The payment methods allowed when ordering from the organisation that fulfills the order                                                                                                                                  | [<br/>"CASH",<br/>"CARD"<br/>]                                                                                                                                                                                           |
| `deliveryMethods`                                                                                                                                                                                                        | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderDeliveryMethod](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-delivery-method.md)[]          | :heavy_minus_sign:                                                                                                                                                                                                       | The order's delivery methods. Applicable only if supply_method is delivery                                                                                                                                               |                                                                                                                                                                                                                          |
| `creatives`                                                                                                                                                                                                              | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderCreative](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-creative.md)[]                       | :heavy_minus_sign:                                                                                                                                                                                                       | Details about creatives. A creative is an object that contains all the data required for visually rendering an image responsively, such as the initial image and a number of scale versions of it (srcset)               |                                                                                                                                                                                                                          |