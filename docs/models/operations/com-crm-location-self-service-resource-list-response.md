# ComCrmLocationSelfServiceResourceListResponse

OK

## Example Usage

```typescript
import { ComCrmLocationSelfServiceResourceListResponse } from "crmcom/models/operations";

let value: ComCrmLocationSelfServiceResourceListResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "CRM",
      description: "CRM organisation for orders",
      address: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        addressLine1: "Elia Papakyriakou",
        addressLine2: "7 Tower Stars",
        stateProvinceCounty: "Egkomi",
        townCity: "Nicosia",
        postalCode: "2000",
        countryCode: "CYP",
        lat: 12.16,
        lon: 112.16,
        distance: 11,
        googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
      },
      openingHours: [
        {
          open: "12:45",
          close: "19:45",
        },
      ],
      contactInfo: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          name: "Main Office",
          value: "johndoe@deliciousfood.com",
          countryCode: "CYP",
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
      orderCatalogs: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          displayName: "Drinks Menu",
          timeAvailability: [
            {
              startTime: "09:00",
              endTime: "17:00",
            },
          ],
          supplyMethods: [
            "DELIVERY",
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
      tags: [
        {
          name: "Accounting",
        },
      ],
      customFields: [
        {
          key: "back_office",
          value: "0001-12345",
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                       | Type                                                                                                                                        | Required                                                                                                                                    | Description                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                    | [operations.ComCrmLocationSelfServiceResourceListPaging](../../models/operations/com-crm-location-self-service-resource-list-paging.md)     | :heavy_minus_sign:                                                                                                                          | N/A                                                                                                                                         |
| `content`                                                                                                                                   | [operations.ComCrmLocationSelfServiceResourceListContent](../../models/operations/com-crm-location-self-service-resource-list-content.md)[] | :heavy_minus_sign:                                                                                                                          | N/A                                                                                                                                         |