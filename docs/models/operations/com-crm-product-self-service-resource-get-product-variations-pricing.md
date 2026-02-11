# ComCrmProductSelfServiceResourceGetProductVariationsPricing

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductVariationsPricing } from "crmcom/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductVariationsPricing = {
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
};
```

## Fields

| Field                                                                                                                                                                                | Type                                                                                                                                                                                 | Required                                                                                                                                                                             | Description                                                                                                                                                                          | Example                                                                                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                                 | *string*                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                   | The entity identifier                                                                                                                                                                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                 |
| `price`                                                                                                                                                                              | *number*                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                   | Price                                                                                                                                                                                | 9.99                                                                                                                                                                                 |
| `label`                                                                                                                                                                              | *string*                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                   | Price label                                                                                                                                                                          | 9.99                                                                                                                                                                                 |
| `currencyCode`                                                                                                                                                                       | [operations.ComCrmProductSelfServiceResourceGetProductVariationsCurrencyCode](../../models/operations/com-crm-product-self-service-resource-get-product-variations-currency-code.md) | :heavy_minus_sign:                                                                                                                                                                   | Currency code                                                                                                                                                                        | EUR                                                                                                                                                                                  |
| `isDefault`                                                                                                                                                                          | *boolean*                                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                                   | Default price                                                                                                                                                                        | true                                                                                                                                                                                 |
| `taxModel`                                                                                                                                                                           | [operations.ComCrmProductSelfServiceResourceGetProductVariationsTaxModel](../../models/operations/com-crm-product-self-service-resource-get-product-variations-tax-model.md)         | :heavy_minus_sign:                                                                                                                                                                   | The tax model of price                                                                                                                                                               | TAX_INCLUSIVE                                                                                                                                                                        |
| `priceModel`                                                                                                                                                                         | [operations.ComCrmProductSelfServiceResourceGetProductVariationsPriceModel](../../models/operations/com-crm-product-self-service-resource-get-product-variations-price-model.md)     | :heavy_minus_sign:                                                                                                                                                                   | The price model of price                                                                                                                                                             | FLAT                                                                                                                                                                                 |
| `supplyMethod`                                                                                                                                                                       | [operations.ComCrmProductSelfServiceResourceGetProductVariationsSupplyMethod](../../models/operations/com-crm-product-self-service-resource-get-product-variations-supply-method.md) | :heavy_minus_sign:                                                                                                                                                                   | Defines the order’ supply method                                                                                                                                                     | DELIVERY                                                                                                                                                                             |
| `salesModel`                                                                                                                                                                         | [operations.ComCrmProductSelfServiceResourceGetProductVariationsSalesModel](../../models/operations/com-crm-product-self-service-resource-get-product-variations-sales-model.md)     | :heavy_minus_sign:                                                                                                                                                                   | The sales model unique identifier which will enable the user to choose one of the configured sales model types for the product                                                       | DELIVERY                                                                                                                                                                             |
| `orderQueue`                                                                                                                                                                         | [operations.ComCrmProductSelfServiceResourceGetProductVariationsOrderQueue](../../models/operations/com-crm-product-self-service-resource-get-product-variations-order-queue.md)     | :heavy_minus_sign:                                                                                                                                                                   | N/A                                                                                                                                                                                  |                                                                                                                                                                                      |
| `priceTerms`                                                                                                                                                                         | [operations.ComCrmProductSelfServiceResourceGetProductVariationsPriceTerms](../../models/operations/com-crm-product-self-service-resource-get-product-variations-price-terms.md)     | :heavy_minus_sign:                                                                                                                                                                   | price terms                                                                                                                                                                          |                                                                                                                                                                                      |
| `tiers`                                                                                                                                                                              | [operations.ComCrmProductSelfServiceResourceGetProductVariationsTier](../../models/operations/com-crm-product-self-service-resource-get-product-variations-tier.md)[]                | :heavy_minus_sign:                                                                                                                                                                   | List of tiered prices. Applicable only for Tiered/Volume/Stairstep pricing models                                                                                                    |                                                                                                                                                                                      |