# ComCrmProductSelfServiceResourceGetProductComponentsProduct

## Example Usage

```typescript
import { ComCrmProductSelfServiceResourceGetProductComponentsProduct } from "crmcom/models/operations";

let value: ComCrmProductSelfServiceResourceGetProductComponentsProduct = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  pricing: [
    {
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
  characteristics: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      key: "colour",
      value: "RED",
      label: "RED",
      mandatory: true,
    },
  ],
  customFields: [
    {
      key: "back_office",
      value: "0001-12345",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                                        | Type                                                                                                                                                                                         | Required                                                                                                                                                                                     | Description                                                                                                                                                                                  | Example                                                                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                         | *string*                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                           | The entity identifier                                                                                                                                                                        | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                         |
| `sku`                                                                                                                                                                                        | *string*                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                           | N/A                                                                                                                                                                                          |                                                                                                                                                                                              |
| `name`                                                                                                                                                                                       | *string*                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                           | N/A                                                                                                                                                                                          |                                                                                                                                                                                              |
| `description`                                                                                                                                                                                | *string*                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                           | N/A                                                                                                                                                                                          |                                                                                                                                                                                              |
| `availability`                                                                                                                                                                               | [operations.ComCrmProductSelfServiceResourceGetProductComponentsAvailability](../../models/operations/com-crm-product-self-service-resource-get-product-components-availability.md)          | :heavy_minus_sign:                                                                                                                                                                           | N/A                                                                                                                                                                                          |                                                                                                                                                                                              |
| `isIncluded`                                                                                                                                                                                 | *boolean*                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                           | N/A                                                                                                                                                                                          |                                                                                                                                                                                              |
| `pricing`                                                                                                                                                                                    | [operations.ComCrmProductSelfServiceResourceGetProductComponentsPricing](../../models/operations/com-crm-product-self-service-resource-get-product-components-pricing.md)[]                  | :heavy_minus_sign:                                                                                                                                                                           | N/A                                                                                                                                                                                          |                                                                                                                                                                                              |
| `creatives`                                                                                                                                                                                  | [operations.ComCrmProductSelfServiceResourceGetProductComponentsCreative](../../models/operations/com-crm-product-self-service-resource-get-product-components-creative.md)[]                | :heavy_minus_sign:                                                                                                                                                                           | N/A                                                                                                                                                                                          |                                                                                                                                                                                              |
| `stockInformation`                                                                                                                                                                           | [operations.ComCrmProductSelfServiceResourceGetProductComponentsStockInformation](../../models/operations/com-crm-product-self-service-resource-get-product-components-stock-information.md) | :heavy_minus_sign:                                                                                                                                                                           | The product variant stock information (returned only if include_stock is set to true)                                                                                                        |                                                                                                                                                                                              |
| `characteristics`                                                                                                                                                                            | [operations.ComCrmProductSelfServiceResourceGetProductComponentsCharacteristic](../../models/operations/com-crm-product-self-service-resource-get-product-components-characteristic.md)[]    | :heavy_minus_sign:                                                                                                                                                                           | List of product characteristics and their values                                                                                                                                             |                                                                                                                                                                                              |
| `customFields`                                                                                                                                                                               | [operations.ComCrmProductSelfServiceResourceGetProductComponentsCustomField](../../models/operations/com-crm-product-self-service-resource-get-product-components-custom-field.md)[]         | :heavy_minus_sign:                                                                                                                                                                           | A list of custom fields values                                                                                                                                                               |                                                                                                                                                                                              |