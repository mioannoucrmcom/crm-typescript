# InvoiceEstimateItem

## Example Usage

```typescript
import { InvoiceEstimateItem } from "crm/models/operations";

let value: InvoiceEstimateItem = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  quantity: 2,
  unitPrice: 10,
  netAmount: 20.5,
  taxAmount: 10,
  subTotal: 200.5,
  period: {
    from: 1651172405,
    to: 1653764405,
  },
  discount: {
    discountAmount: 20.5,
    discountPercentage: 10,
  },
  product: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    sku: "CBL-54455",
    name: "Cable",
    classification: "TRACEABLE_PHYSICAL_GOOD",
    isStockable: false,
  },
  bundleProduct: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    sku: "CBL-54455",
    name: "Cable",
    classification: "TRACEABLE_PHYSICAL_GOOD",
    isStockable: false,
  },
  appliedTaxes: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      taxRate: {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "VAT",
        taxCode: "VAT",
      },
      taxAmount: 1.5,
      taxExemptReason: "PRODUCT",
    },
  ],
  pricing: 11.99,
  inStock: 1,
};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             | Example                                                                                                                 |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                    | *string*                                                                                                                | :heavy_minus_sign:                                                                                                      | The entity identifier                                                                                                   | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                    |
| `quantity`                                                                                                              | *number*                                                                                                                | :heavy_minus_sign:                                                                                                      | The quantity of the product                                                                                             | 2                                                                                                                       |
| `unitPrice`                                                                                                             | *number*                                                                                                                | :heavy_minus_sign:                                                                                                      | The price per unit of the product                                                                                       | 10                                                                                                                      |
| `netAmount`                                                                                                             | *number*                                                                                                                | :heavy_minus_sign:                                                                                                      | The net amount                                                                                                          | 20.5                                                                                                                    |
| `taxAmount`                                                                                                             | *number*                                                                                                                | :heavy_minus_sign:                                                                                                      | Total taxed amount for this product                                                                                     | 10                                                                                                                      |
| `subTotal`                                                                                                              | *number*                                                                                                                | :heavy_minus_sign:                                                                                                      | The sub total of the financial transaction line                                                                         | 200.5                                                                                                                   |
| `period`                                                                                                                | [operations.ItemPeriod](../../models/operations/item-period.md)                                                         | :heavy_minus_sign:                                                                                                      | Invoiced period applicable only when invoicing a termed service.                                                        |                                                                                                                         |
| `discount`                                                                                                              | [operations.InvoiceEstimateItemDiscount](../../models/operations/invoice-estimate-item-discount.md)                     | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `product`                                                                                                               | [operations.InvoiceEstimateProduct](../../models/operations/invoice-estimate-product.md)                                | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `bundleProduct`                                                                                                         | [operations.ItemBundleProduct](../../models/operations/item-bundle-product.md)                                          | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `appliedTaxes`                                                                                                          | [operations.ItemAppliedTax](../../models/operations/item-applied-tax.md)[]                                              | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |                                                                                                                         |
| `pricing`                                                                                                               | *number*                                                                                                                | :heavy_minus_sign:                                                                                                      | The price of the product as this is configured in the product catalog (including tax or not depending on the tax model) | 11.99                                                                                                                   |
| `inStock`                                                                                                               | *number*                                                                                                                | :heavy_minus_sign:                                                                                                      | The quantity of the product that is available for the customer to order                                                 | 1                                                                                                                       |