# ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationResponse

OK

## Example Usage

```typescript
import { ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationResponse } from "crm/models/operations";

let value:
  ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationResponse =
    {
      paging: {
        page: 2,
        size: 20,
        total: 5124,
        hasMore: true,
      },
      content: [
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
                  url:
                    "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
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
        },
      ],
    };
```

## Fields

| Field                                                                                                                                                                                                            | Type                                                                                                                                                                                                             | Required                                                                                                                                                                                                         | Description                                                                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                                                         | [operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationPaging](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-paging.md)     | :heavy_minus_sign:                                                                                                                                                                                               | N/A                                                                                                                                                                                                              |
| `content`                                                                                                                                                                                                        | [operations.ComCrmServiceRecommendationSelfServiceResourceGetServiceRecommendationContent](../../models/operations/com-crm-service-recommendation-self-service-resource-get-service-recommendation-content.md)[] | :heavy_minus_sign:                                                                                                                                                                                               | N/A                                                                                                                                                                                                              |