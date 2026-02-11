# UpsellPricing

## Example Usage

```typescript
import { UpsellPricing } from "crmcom/models/operations";

let value: UpsellPricing = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  currencyCode: "EUR",
  taxModel: "TAX_INCLUSIVE",
  tiers: {
    upperTier: 1,
    numberOfTiers: 3,
  },
  billingPeriod: {
    duration: 2,
    uot: "MONTH",
  },
  measurementUnit: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "Gigabytes",
    displayName: "GB",
  },
  accessPeriod: {
    startDate: 1612953199,
    endDate: 1612953199,
  },
  orderQueue: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Universal Name",
  },
};
```

## Fields

| Field                                                                                                                         | Type                                                                                                                          | Required                                                                                                                      | Description                                                                                                                   | Example                                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                          | *string*                                                                                                                      | :heavy_minus_sign:                                                                                                            | The entity identifier                                                                                                         | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                          |
| `priceModel`                                                                                                                  | [operations.UpsellPriceModel](../../models/operations/upsell-price-model.md)                                                  | :heavy_minus_sign:                                                                                                            | The pricing model:<br/> * `FLAT`<br/> * `TIERED`<br/> * `VOLUME`<br/> * `STAIRSTEP`                                       |                                                                                                                               |
| `currencyCode`                                                                                                                | [operations.UpsellCurrencyCode](../../models/operations/upsell-currency-code.md)                                              | :heavy_minus_sign:                                                                                                            | Currency code based on ISO 4217 standard                                                                                      | EUR                                                                                                                           |
| `taxModel`                                                                                                                    | [operations.UpsellTaxModel](../../models/operations/upsell-tax-model.md)                                                      | :heavy_minus_sign:                                                                                                            | Defines whether the price is tax inclusive or not. Defaults to the system's Taxation setting                                  | TAX_INCLUSIVE                                                                                                                 |
| `price`                                                                                                                       | *number*                                                                                                                      | :heavy_minus_sign:                                                                                                            | The product's price. For Tiered/Volume and Stairstep pricing models, the first range's price is returned.                     |                                                                                                                               |
| `tiers`                                                                                                                       | [operations.UpsellTiers](../../models/operations/upsell-tiers.md)                                                             | :heavy_minus_sign:                                                                                                            | Available only Tiered, Volume and Stairstep pricing models. Only the first tier range is returned that has the returned price |                                                                                                                               |
| `billingPeriod`                                                                                                               | [operations.UpsellBillingPeriod](../../models/operations/upsell-billing-period.md)                                            | :heavy_minus_sign:                                                                                                            | The billing period mapped to the specified price. Applicable only for termed and one-time services only.                      |                                                                                                                               |
| `measurementUnit`                                                                                                             | [operations.UpsellMeasurementUnit](../../models/operations/upsell-measurement-unit.md)                                        | :heavy_minus_sign:                                                                                                            | Applicable only for Usage service to show the unit per which the price is applied                                             |                                                                                                                               |
| `accessPeriod`                                                                                                                | [operations.UpsellAccessPeriod](../../models/operations/upsell-access-period.md)                                              | :heavy_minus_sign:                                                                                                            | The period of time that service will be accessible. Applicable only for one-time services                                     |                                                                                                                               |
| `orderQueue`                                                                                                                  | [operations.UpsellOrderQueue](../../models/operations/upsell-order-queue.md)                                                  | :heavy_minus_sign:                                                                                                            | Details about the related product order queue                                                                                 |                                                                                                                               |