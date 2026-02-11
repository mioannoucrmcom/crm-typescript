# DeliveryServiceProvider

## Example Usage

```typescript
import { DeliveryServiceProvider } from "crmcom/models/operations";

let value: DeliveryServiceProvider = {
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
          url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                                      | Type                                                                                                                                                                                                       | Required                                                                                                                                                                                                   | Description                                                                                                                                                                                                | Example                                                                                                                                                                                                    |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                                       | *string*                                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                         | The delivery service provider identifier                                                                                                                                                                   | e283a863-18e1-7cae-48c4-7433bf28cf97                                                                                                                                                                       |
| `name`                                                                                                                                                                                                     | *string*                                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                                         | The delivery service provider name                                                                                                                                                                         | ACS                                                                                                                                                                                                        |
| `creatives`                                                                                                                                                                                                | [operations.DeliveryServiceProviderCreative](../../models/operations/delivery-service-provider-creative.md)[]                                                                                              | :heavy_minus_sign:                                                                                                                                                                                         | Details about creatives. A creative is an object that contains all the data required for visually rendering an image responsively, such as the initial image and a number of scale versions of it (srcset) |                                                                                                                                                                                                            |