# ComCrmLocationSelfServiceResourceListContent

## Example Usage

```typescript
import { ComCrmLocationSelfServiceResourceListContent } from "crm/models/operations";

let value: ComCrmLocationSelfServiceResourceListContent = {
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
              url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
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
};
```

## Fields

| Field                                                                                                                                                  | Type                                                                                                                                                   | Required                                                                                                                                               | Description                                                                                                                                            | Example                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                   | *string*                                                                                                                                               | :heavy_minus_sign:                                                                                                                                     | The entity identifier                                                                                                                                  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                   |
| `name`                                                                                                                                                 | *string*                                                                                                                                               | :heavy_minus_sign:                                                                                                                                     | The organisation name                                                                                                                                  | CRM                                                                                                                                                    |
| `description`                                                                                                                                          | *string*                                                                                                                                               | :heavy_minus_sign:                                                                                                                                     | The organisation description                                                                                                                           | CRM organisation for orders                                                                                                                            |
| `address`                                                                                                                                              | [operations.ComCrmLocationSelfServiceResourceListAddress](../../models/operations/com-crm-location-self-service-resource-list-address.md)              | :heavy_minus_sign:                                                                                                                                     | The organisation address                                                                                                                               |                                                                                                                                                        |
| `openingHours`                                                                                                                                         | [operations.ComCrmLocationSelfServiceResourceListOpeningHour](../../models/operations/com-crm-location-self-service-resource-list-opening-hour.md)[]   | :heavy_minus_sign:                                                                                                                                     | The organisation opening hours for the current day                                                                                                     |                                                                                                                                                        |
| `contactInfo`                                                                                                                                          | [operations.ComCrmLocationSelfServiceResourceListContactInfo](../../models/operations/com-crm-location-self-service-resource-list-contact-info.md)[]   | :heavy_minus_sign:                                                                                                                                     | The organisation contact information                                                                                                                   |                                                                                                                                                        |
| `creatives`                                                                                                                                            | [operations.ComCrmLocationSelfServiceResourceListCreative](../../models/operations/com-crm-location-self-service-resource-list-creative.md)[]          | :heavy_minus_sign:                                                                                                                                     | Creatives images for marketing includes the primary image and scaled versions to create a srcset                                                       |                                                                                                                                                        |
| `orderCatalogs`                                                                                                                                        | [operations.ComCrmLocationSelfServiceResourceListOrderCatalog](../../models/operations/com-crm-location-self-service-resource-list-order-catalog.md)[] | :heavy_minus_sign:                                                                                                                                     | The order catalogs applicable for the organisation                                                                                                     |                                                                                                                                                        |
| `tags`                                                                                                                                                 | [operations.ComCrmLocationSelfServiceResourceListTag](../../models/operations/com-crm-location-self-service-resource-list-tag.md)[]                    | :heavy_minus_sign:                                                                                                                                     | The tags of the organisation                                                                                                                           | [<br/>{<br/>"name": "Accounting"<br/>}<br/>]                                                                                                           |
| `customFields`                                                                                                                                         | [operations.ComCrmLocationSelfServiceResourceListCustomField](../../models/operations/com-crm-location-self-service-resource-list-custom-field.md)[]   | :heavy_minus_sign:                                                                                                                                     | The organisation custom fields                                                                                                                         |                                                                                                                                                        |