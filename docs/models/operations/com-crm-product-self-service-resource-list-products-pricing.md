# ComCrmProductSelfServiceResourceListProductsPricing

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceListProductsPricing } from "crm/models/operations";

let value: ComCrmProductSelfServiceResourceListProductsPricing = {
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
};
```

## Fields

| Field                                                                                                                                                               | Type                                                                                                                                                                | Required                                                                                                                                                            | Description                                                                                                                                                         | Example                                                                                                                                                             |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                | *string*                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                  | The entity identifier                                                                                                                                               | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                |
| `price`                                                                                                                                                             | *number*                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                  | Price                                                                                                                                                               | 9.99                                                                                                                                                                |
| `label`                                                                                                                                                             | *string*                                                                                                                                                            | :heavy_minus_sign:                                                                                                                                                  | Price label                                                                                                                                                         | 9.99                                                                                                                                                                |
| `currencyCode`                                                                                                                                                      | [operations.ComCrmProductSelfServiceResourceListProductsCurrencyCode](../../models/operations/com-crm-product-self-service-resource-list-products-currency-code.md) | :heavy_minus_sign:                                                                                                                                                  | Currency code                                                                                                                                                       | EUR                                                                                                                                                                 |
| `isDefault`                                                                                                                                                         | *boolean*                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                  | Default price                                                                                                                                                       | true                                                                                                                                                                |
| `taxModel`                                                                                                                                                          | [operations.ComCrmProductSelfServiceResourceListProductsTaxModel](../../models/operations/com-crm-product-self-service-resource-list-products-tax-model.md)         | :heavy_minus_sign:                                                                                                                                                  | The tax model of price                                                                                                                                              | TAX_INCLUSIVE                                                                                                                                                       |
| `priceModel`                                                                                                                                                        | [operations.ComCrmProductSelfServiceResourceListProductsPriceModel](../../models/operations/com-crm-product-self-service-resource-list-products-price-model.md)     | :heavy_minus_sign:                                                                                                                                                  | The price model of price                                                                                                                                            | FLAT                                                                                                                                                                |
| `supplyMethod`                                                                                                                                                      | [operations.ComCrmProductSelfServiceResourceListProductsSupplyMethod](../../models/operations/com-crm-product-self-service-resource-list-products-supply-method.md) | :heavy_minus_sign:                                                                                                                                                  | Defines the order’ supply method                                                                                                                                    | DELIVERY                                                                                                                                                            |
| `salesModel`                                                                                                                                                        | [operations.ComCrmProductSelfServiceResourceListProductsSalesModel](../../models/operations/com-crm-product-self-service-resource-list-products-sales-model.md)     | :heavy_minus_sign:                                                                                                                                                  | The sales model unique identifier which will enable the user to choose one of the configured sales model types for the product                                      | DELIVERY                                                                                                                                                            |
| `orderQueue`                                                                                                                                                        | [operations.ComCrmProductSelfServiceResourceListProductsOrderQueue](../../models/operations/com-crm-product-self-service-resource-list-products-order-queue.md)     | :heavy_minus_sign:                                                                                                                                                  | N/A                                                                                                                                                                 |                                                                                                                                                                     |
| `priceTerms`                                                                                                                                                        | [operations.ComCrmProductSelfServiceResourceListProductsPriceTerms](../../models/operations/com-crm-product-self-service-resource-list-products-price-terms.md)     | :heavy_minus_sign:                                                                                                                                                  | price terms                                                                                                                                                         |                                                                                                                                                                     |
| `tiers`                                                                                                                                                             | [operations.ComCrmProductSelfServiceResourceListProductsTier](../../models/operations/com-crm-product-self-service-resource-list-products-tier.md)[]                | :heavy_minus_sign:                                                                                                                                                  | List of tiered prices. Applicable only for Tiered/Volume/Stairstep pricing models                                                                                   |                                                                                                                                                                     |