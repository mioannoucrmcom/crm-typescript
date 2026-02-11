# ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderResponse

OK

## Example Usage

```typescript
import { ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderResponse } from "crm/models/operations";

let value:
  ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderResponse = {
    fulfilledBy: [
      {
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
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
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

| Field                                                                                                                                                                                                     | Type                                                                                                                                                                                                      | Required                                                                                                                                                                                                  | Description                                                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `fulfilledBy`                                                                                                                                                                                             | [operations.ComCrmEstimateOrderFulfillmentSelfServiceResourceEstimateOrderFulfilledBy](../../models/operations/com-crm-estimate-order-fulfillment-self-service-resource-estimate-order-fulfilled-by.md)[] | :heavy_minus_sign:                                                                                                                                                                                        | Details about the organisation (business/merchant/venues) that will fulfill the order                                                                                                                     |