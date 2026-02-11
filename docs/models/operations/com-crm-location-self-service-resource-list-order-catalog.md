# ComCrmLocationSelfServiceResourceListOrderCatalog

## Example Usage

```typescript
import { ComCrmLocationSelfServiceResourceListOrderCatalog } from "crm/models/operations";

let value: ComCrmLocationSelfServiceResourceListOrderCatalog = {
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
};
```

## Fields

| Field                                                                                                                                                                            | Type                                                                                                                                                                             | Required                                                                                                                                                                         | Description                                                                                                                                                                      | Example                                                                                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                             | *string*                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                               | The entity identifier                                                                                                                                                            | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                             |
| `displayName`                                                                                                                                                                    | *string*                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                               | The order catalog display name                                                                                                                                                   | Drinks Menu                                                                                                                                                                      |
| `timeAvailability`                                                                                                                                                               | [operations.ComCrmLocationSelfServiceResourceListTimeAvailability](../../models/operations/com-crm-location-self-service-resource-list-time-availability.md)[]                   | :heavy_minus_sign:                                                                                                                                                               | Details about the catalog time availability                                                                                                                                      |                                                                                                                                                                                  |
| `supplyMethods`                                                                                                                                                                  | [operations.ComCrmLocationSelfServiceResourceListOrderCatalogSupplyMethod](../../models/operations/com-crm-location-self-service-resource-list-order-catalog-supply-method.md)[] | :heavy_minus_sign:                                                                                                                                                               | The supported supply methods of the order catalog                                                                                                                                |                                                                                                                                                                                  |
| `creatives`                                                                                                                                                                      | [operations.ComCrmLocationSelfServiceResourceListOrderCatalogCreative](../../models/operations/com-crm-location-self-service-resource-list-order-catalog-creative.md)[]          | :heavy_minus_sign:                                                                                                                                                               | Creatives images for marketing includes the primary image and scaled versions to create a srcset                                                                                 |                                                                                                                                                                                  |