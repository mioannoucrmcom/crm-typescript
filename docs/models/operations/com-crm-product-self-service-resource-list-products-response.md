# ComCrmProductSelfServiceResourceListProductsResponse

OK

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceListProductsResponse } from "crm/models/operations";

let value: ComCrmProductSelfServiceResourceListProductsResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      sku: "ABC12345",
      name: "Movies",
      description: "Unlimited  movies",
      classification: "TRACEABLE_PHYSICAL_GOOD",
      components: 3,
      variants: 3,
      numberOfCharacteristics: 2,
      availability: "ENABLED",
      owner: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
      },
      isModifier: true,
      negativeBalanceAllowed: true,
      isProvisionable: true,
      isStockable: true,
      instanceModel: "QUANTITY_BASED",
      characteristics: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          key: "colour",
          value: "RED",
          label: "RED",
          mandatory: true,
        },
      ],
      pricing: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          price: 9.99,
          label: "9.99",
          currencyCode: "EUR",
          isDefault: true,
          taxModel: "TAX_INCLUSIVE",
          priceModel: "FLAT",
          supplyMethod: "DELIVERY",
          salesModel: {
            id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
            name: "Universal Name",
          },
          orderQueue: {
            id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
            name: "Universal Name",
          },
          priceTerms: {
            billingPeriod: {
              duration: 2,
              uot: "OVERALL",
            },
            trialPeriod: {
              duration: 2,
              uot: "HOUR",
            },
            accessPeriod: {
              startDate: 1612953199,
              endDate: 1612953199,
            },
            billingModel: "PRE_BILL",
            contractPeriod: {
              duration: 2,
              uot: "MINUTE",
            },
            rentalService: {
              id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
              name: "Universal Name",
              sku: "S0001",
            },
            valueType: "VARIABLE",
          },
          tiers: [
            {
              id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
              lowerTier: 1,
              upperTier: 5,
              price: 8.99,
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
      customFields: [
        {
          key: "back_office",
          value: "0001-12345",
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

| Field                                                                                                                                                      | Type                                                                                                                                                       | Required                                                                                                                                                   | Description                                                                                                                                                |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                   | [operations.ComCrmProductSelfServiceResourceListProductsPaging](../../models/operations/com-crm-product-self-service-resource-list-products-paging.md)     | :heavy_minus_sign:                                                                                                                                         | N/A                                                                                                                                                        |
| `content`                                                                                                                                                  | [operations.ComCrmProductSelfServiceResourceListProductsContent](../../models/operations/com-crm-product-self-service-resource-list-products-content.md)[] | :heavy_minus_sign:                                                                                                                                         | N/A                                                                                                                                                        |