# ComCrmProductSelfServiceResourceGetProductComponentsPricing

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductComponentsPricing } from "crmcom/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductComponentsPricing = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  price: 9.99,
  label: "9.99",
  currency: "EUR",
  taxModel: "TAX_INCLUSIVE",
  rateModel: "FLAT",
  supplyMethod: "DELIVERY",
  taxes: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "vat",
      percentage: 8.88,
      taxCode: "VAT",
    },
  ],
  priceTerms: [
    {
      billingPeriod: {
        duration: 2,
        uot: "MINUTE",
      },
      trialPeriod: {
        duration: 2,
        uot: "MINUTE",
      },
      priceModel: "VARIABLE",
      billingModel: "PRE_BILL",
      contractPeriod: {
        duration: 2,
        uot: "YEAR",
      },
      rentalService: {
        id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
        name: "Universal Name",
        sku: "S0001",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                | Type                                                                                                                                                                                 | Required                                                                                                                                                                             | Description                                                                                                                                                                          | Example                                                                                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                                 | *string*                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                   | The entity identifier                                                                                                                                                                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                 |
| `price`                                                                                                                                                                              | *number*                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                   | the price                                                                                                                                                                            | 9.99                                                                                                                                                                                 |
| `label`                                                                                                                                                                              | *string*                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                   | the price label                                                                                                                                                                      | 9.99                                                                                                                                                                                 |
| `currency`                                                                                                                                                                           | [operations.ComCrmProductSelfServiceResourceGetProductComponentsCurrency](../../models/operations/com-crm-product-self-service-resource-get-product-components-currency.md)          | :heavy_minus_sign:                                                                                                                                                                   | the currency code of price                                                                                                                                                           | EUR                                                                                                                                                                                  |
| `taxModel`                                                                                                                                                                           | [operations.ComCrmProductSelfServiceResourceGetProductComponentsTaxModel](../../models/operations/com-crm-product-self-service-resource-get-product-components-tax-model.md)         | :heavy_minus_sign:                                                                                                                                                                   | the tax model of price                                                                                                                                                               | TAX_INCLUSIVE                                                                                                                                                                        |
| `rateModel`                                                                                                                                                                          | [operations.RateModel](../../models/operations/rate-model.md)                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                   | the rate model of price                                                                                                                                                              | FLAT                                                                                                                                                                                 |
| `supplyMethod`                                                                                                                                                                       | [operations.ComCrmProductSelfServiceResourceGetProductComponentsSupplyMethod](../../models/operations/com-crm-product-self-service-resource-get-product-components-supply-method.md) | :heavy_minus_sign:                                                                                                                                                                   | Defines the order’ supply method                                                                                                                                                     | DELIVERY                                                                                                                                                                             |
| `taxes`                                                                                                                                                                              | [operations.Tax](../../models/operations/tax.md)[]                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                   | price taxes                                                                                                                                                                          |                                                                                                                                                                                      |
| `priceTerms`                                                                                                                                                                         | [operations.PriceTerm](../../models/operations/price-term.md)[]                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                   | price terms                                                                                                                                                                          |                                                                                                                                                                                      |
| `tiers`                                                                                                                                                                              | [operations.ComCrmProductSelfServiceResourceGetProductComponentsTier](../../models/operations/com-crm-product-self-service-resource-get-product-components-tier.md)[]                | :heavy_minus_sign:                                                                                                                                                                   | List of prices per range. Applicable only for Tiers/Volume/Stairstep pricing models                                                                                                  |                                                                                                                                                                                      |