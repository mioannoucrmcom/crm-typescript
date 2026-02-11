# ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationContent

## Example Usage

```typescript
import { ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationContent } from "crmcom/models/operations";

let value:
  ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationContent =
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      composition: "FLAT",
      instanceModel: "QUANTITY_BASED",
      prices: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          currencyCode: "EUR",
          taxModel: "TAX_INCLUSIVE",
          priceTerms: {
            billingModel: "PRE_BILL",
            billingPeriod: {
              duration: 2,
              uot: "HOUR",
            },
            trialPeriod: {
              duration: 2,
              uot: "HOUR",
            },
            contractPeriod: {
              duration: 2,
              uot: "HOUR",
            },
          },
        },
      ],
      components: [
        {
          itemType: "PRODUCT",
          itemId: "8c939607-2262-544d-99ef-4634c6e8836d",
          name: "TV Services",
          mandatory: true,
          priceInclusive: true,
          minimumQuantity: 1,
          maximumQuantity: 3,
          price: {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
            price: 9.99,
            outContractPrice: 11.99,
            currencyCode: "EUR",
            taxModel: "TAX_INCLUSIVE",
          },
          products: [
            {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              pricing: {
                id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
                price: 9.99,
                outContractPrice: 11.99,
                currencyCode: "EUR",
                taxModel: "TAX_INCLUSIVE",
              },
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
      includedOneTimeServices: [
        {
          id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
          name: "Universal Name",
          sku: "S0001",
        },
      ],
    };
```

## Fields

| Field                                                                                                                                                                                                                                                                                            | Type                                                                                                                                                                                                                                                                                             | Required                                                                                                                                                                                                                                                                                         | Description                                                                                                                                                                                                                                                                                      | Example                                                                                                                                                                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                                                                                                                                             | *string*                                                                                                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                                                                                               | The entity identifier                                                                                                                                                                                                                                                                            | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                                                                                                             |
| `sku`                                                                                                                                                                                                                                                                                            | *string*                                                                                                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                                                                                               | Product SKU                                                                                                                                                                                                                                                                                      |                                                                                                                                                                                                                                                                                                  |
| `name`                                                                                                                                                                                                                                                                                           | *string*                                                                                                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                                                                                               | Product name                                                                                                                                                                                                                                                                                     |                                                                                                                                                                                                                                                                                                  |
| `description`                                                                                                                                                                                                                                                                                    | *string*                                                                                                                                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                                                                                                                               | Product descriptiption                                                                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                  |
| `composition`                                                                                                                                                                                                                                                                                    | [operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationComposition](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-composition.md)                                                                           | :heavy_minus_sign:                                                                                                                                                                                                                                                                               | Product Composition                                                                                                                                                                                                                                                                              | FLAT                                                                                                                                                                                                                                                                                             |
| `instanceModel`                                                                                                                                                                                                                                                                                  | [operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationInstanceModel](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-instance-model.md)                                                                      | :heavy_minus_sign:                                                                                                                                                                                                                                                                               | Determines whether a service is managed as a single quantity or as separate, independently managed instances on a subscription                                                                                                                                                                   | QUANTITY_BASED                                                                                                                                                                                                                                                                                   |
| `prices`                                                                                                                                                                                                                                                                                         | [operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationPrice](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-price.md)[]                                                                                     | :heavy_minus_sign:                                                                                                                                                                                                                                                                               | List of applicable prices for the recommended service                                                                                                                                                                                                                                            |                                                                                                                                                                                                                                                                                                  |
| `components`                                                                                                                                                                                                                                                                                     | [operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationComponent](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-component.md)[]                                                                             | :heavy_minus_sign:                                                                                                                                                                                                                                                                               | Returned only when the recommended service is classified as a Flexible bundle                                                                                                                                                                                                                    |                                                                                                                                                                                                                                                                                                  |
| `creatives`                                                                                                                                                                                                                                                                                      | [operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationCreative](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-creative.md)[]                                                                               | :heavy_minus_sign:                                                                                                                                                                                                                                                                               | Details about creatives. A creative is an object that contains all the data required for visually rendering an image responsively, such as the initial image and a number of scale versions of it (srcset)                                                                                       |                                                                                                                                                                                                                                                                                                  |
| `includedOneTimeServices`                                                                                                                                                                                                                                                                        | [operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationIncludedOneTimeService](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-included-one-time-service.md)[]                                                | :heavy_minus_sign:                                                                                                                                                                                                                                                                               | A list of one-time services which extend the behaviour of a termed service product so whenever the termed service is added/renewed, then all related one-time service are added to the same subscription. Only one-time services can be specified and applicable only for flat, termed services. |                                                                                                                                                                                                                                                                                                  |