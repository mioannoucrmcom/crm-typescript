# ComCrmProductSelfServiceResourceGetProductVariationsResponse

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductVariationsResponse } from "crm/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductVariationsResponse = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  sku: "ABC12345",
  name: "small latte",
  description: "small latte coffee on ice",
  priority: 1,
  classification: "TERMED_SERVICE",
  typeComposition: "FLAT",
  numberOfPrices: 3,
  numberOfCharacteristics: 2,
  type: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "lemonade",
  },
  categories: [
    {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Universal Name",
    },
  ],
  family: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "lemonade",
  },
  brand: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "lemonade",
  },
  composition: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      itemType: "PRODUCT",
      itemId: "8c939607-2262-544d-99ef-4634c6e8836d",
      name: "TV Services",
      sku: "ABC12345",
      mandatory: true,
      minimumQuantity: 1,
      maximumQuantity: 3,
      priceInclusive: true,
      priority: 1,
      defaultModifier: {
        id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
        name: "Universal Name",
        sku: "S0001",
      },
      mandatoryProduct: {
        id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
        name: "Universal Name",
        sku: "S0001",
      },
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
          uot: "HOUR",
        },
        trialPeriod: {
          duration: 2,
          uot: "SECOND",
        },
        accessPeriod: {
          startDate: 1612953199,
          endDate: 1612953199,
        },
        billingModel: "PRE_BILL",
        contractPeriod: {
          duration: 2,
          uot: "OVERALL",
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
  characteristics: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      key: "colour",
      value: "RED",
      label: "RED",
      mandatory: true,
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
  stockInformation: {
    stockBalance: 12,
    reserved: 1,
    inStock: true,
  },
};
```

## Fields

| Field                                                                                                                                                                                                  | Type                                                                                                                                                                                                   | Required                                                                                                                                                                                               | Description                                                                                                                                                                                            | Example                                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                                                   | *string*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | The entity identifier                                                                                                                                                                                  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                   |
| `sku`                                                                                                                                                                                                  | *string*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | Product SKU                                                                                                                                                                                            | ABC12345                                                                                                                                                                                               |
| `name`                                                                                                                                                                                                 | *string*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | Product name                                                                                                                                                                                           | small latte                                                                                                                                                                                            |
| `description`                                                                                                                                                                                          | *string*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | Product description                                                                                                                                                                                    | small latte coffee on ice                                                                                                                                                                              |
| `priority`                                                                                                                                                                                             | *number*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | Product priority                                                                                                                                                                                       | 1                                                                                                                                                                                                      |
| `classification`                                                                                                                                                                                       | [operations.ComCrmProductSelfServiceResourceGetProductVariationsClassification](../../models/operations/com-crm-product-self-service-resource-get-product-variations-classification.md)                | :heavy_minus_sign:                                                                                                                                                                                     | Product classification                                                                                                                                                                                 | TERMED_SERVICE                                                                                                                                                                                         |
| `typeComposition`                                                                                                                                                                                      | [operations.ComCrmProductSelfServiceResourceGetProductVariationsTypeComposition](../../models/operations/com-crm-product-self-service-resource-get-product-variations-type-composition.md)             | :heavy_minus_sign:                                                                                                                                                                                     | Product type composition                                                                                                                                                                               | FLAT                                                                                                                                                                                                   |
| `numberOfPrices`                                                                                                                                                                                       | *number*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | number of prices                                                                                                                                                                                       | 3                                                                                                                                                                                                      |
| `numberOfCharacteristics`                                                                                                                                                                              | *number*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | Number of characteristics                                                                                                                                                                              | 2                                                                                                                                                                                                      |
| `type`                                                                                                                                                                                                 | [operations.ComCrmProductSelfServiceResourceGetProductVariationsType](../../models/operations/com-crm-product-self-service-resource-get-product-variations-type.md)                                    | :heavy_minus_sign:                                                                                                                                                                                     | type of product varriant                                                                                                                                                                               |                                                                                                                                                                                                        |
| `categories`                                                                                                                                                                                           | [operations.ComCrmProductSelfServiceResourceGetProductVariationsCategory](../../models/operations/com-crm-product-self-service-resource-get-product-variations-category.md)[]                          | :heavy_minus_sign:                                                                                                                                                                                     | categories of product varriant                                                                                                                                                                         |                                                                                                                                                                                                        |
| `family`                                                                                                                                                                                               | [operations.ComCrmProductSelfServiceResourceGetProductVariationsFamily](../../models/operations/com-crm-product-self-service-resource-get-product-variations-family.md)                                | :heavy_minus_sign:                                                                                                                                                                                     | family of product varriant                                                                                                                                                                             |                                                                                                                                                                                                        |
| `brand`                                                                                                                                                                                                | [operations.ComCrmProductSelfServiceResourceGetProductVariationsBrand](../../models/operations/com-crm-product-self-service-resource-get-product-variations-brand.md)                                  | :heavy_minus_sign:                                                                                                                                                                                     | brand of product varriant                                                                                                                                                                              |                                                                                                                                                                                                        |
| `composition`                                                                                                                                                                                          | [operations.ComCrmProductSelfServiceResourceGetProductVariationsComposition](../../models/operations/com-crm-product-self-service-resource-get-product-variations-composition.md)[]                    | :heavy_minus_sign:                                                                                                                                                                                     | composition of product varriant                                                                                                                                                                        |                                                                                                                                                                                                        |
| `pricing`                                                                                                                                                                                              | [operations.ComCrmProductSelfServiceResourceGetProductVariationsPricing](../../models/operations/com-crm-product-self-service-resource-get-product-variations-pricing.md)[]                            | :heavy_minus_sign:                                                                                                                                                                                     | List of prices of the variant product. A variant product by default is sold using its Composite product’s price. If the variant product’s needs to be differntiated, then it will have its own price.  |                                                                                                                                                                                                        |
| `characteristics`                                                                                                                                                                                      | [operations.ComCrmProductSelfServiceResourceGetProductVariationsCharacteristic](../../models/operations/com-crm-product-self-service-resource-get-product-variations-characteristic.md)[]              | :heavy_minus_sign:                                                                                                                                                                                     | List of product attributes. The allowed attributes and their allowed values are specified at the Composite product specification. Each variant has a unique combination of these attributes and values |                                                                                                                                                                                                        |
| `creatives`                                                                                                                                                                                            | [operations.ComCrmProductSelfServiceResourceGetProductVariationsCreative](../../models/operations/com-crm-product-self-service-resource-get-product-variations-creative.md)[]                          | :heavy_minus_sign:                                                                                                                                                                                     | A creative is an object that contains all the data required for visually rendering an image responsively. The object contains the initial image and a number of scale versions of it (srcset)          |                                                                                                                                                                                                        |
| `availability`                                                                                                                                                                                         | [operations.ComCrmProductSelfServiceResourceGetProductVariationsAvailability](../../models/operations/com-crm-product-self-service-resource-get-product-variations-availability.md)                    | :heavy_minus_sign:                                                                                                                                                                                     | N/A                                                                                                                                                                                                    |                                                                                                                                                                                                        |
| `stockInformation`                                                                                                                                                                                     | [operations.ComCrmProductSelfServiceResourceGetProductVariationsStockInformation](../../models/operations/com-crm-product-self-service-resource-get-product-variations-stock-information.md)           | :heavy_minus_sign:                                                                                                                                                                                     | The product variant stock information (returned only if include_stock is set to true)                                                                                                                  |                                                                                                                                                                                                        |