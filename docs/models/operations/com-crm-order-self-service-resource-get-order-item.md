# ComCrmOrderSelfServiceResourceGetOrderItem

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceGetOrderItem } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourceGetOrderItem = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  notes: "Lorem Ipsum",
  quantity: 10,
  dispatched: 5,
  invoiced: 2,
  price: 1.7,
  tax: 0.08,
  net: 0.08,
  subTotal: 1.78,
  total: 3.4,
  priceTerms: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    billingPeriod: {
      duration: 1,
      uot: "MONTH",
    },
    autoRenew: true,
    termedPeriodCycles: 5,
    contractPeriod: {
      duration: 1,
      uot: "MONTH",
    },
    trialPeriod: {
      duration: 1,
      uot: "MONTH",
    },
    priceModel: "VARIABLE",
    billingModel: "POST_BILL",
  },
  product: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    sku: "0123-112",
    name: "Decoder",
    classification: "TRACEABLE_PHYSICAL_GOOD",
    isStockable: true,
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
    tags: [
      {
        tagId: "JKGJHFSDJHGDSJHGA",
        name: "Maintenance",
      },
    ],
  },
  taxModel: "TAX_INCLUSIVE",
  devices: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                   | Type                                                                                                                                                    | Required                                                                                                                                                | Description                                                                                                                                             | Example                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                    | *string*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | The entity identifier                                                                                                                                   | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                    |
| `notes`                                                                                                                                                 | *string*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | Order item notes                                                                                                                                        | Lorem Ipsum                                                                                                                                             |
| `quantity`                                                                                                                                              | *number*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | How many items were ordered                                                                                                                             | 10                                                                                                                                                      |
| `dispatched`                                                                                                                                            | *number*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | How many items have been dispatched. Applicable ofor stockable products                                                                                 | 5                                                                                                                                                       |
| `invoiced`                                                                                                                                              | *number*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | How many items have been invoiced so far.Number of invoiced items cannot exceed the number of dispatched items.                                         | 2                                                                                                                                                       |
| `price`                                                                                                                                                 | *number*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | The product's price                                                                                                                                     | 1.7                                                                                                                                                     |
| `tax`                                                                                                                                                   | *number*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | Order item's taxed amount                                                                                                                               | 0.08                                                                                                                                                    |
| `net`                                                                                                                                                   | *number*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | Order item's net amount                                                                                                                                 | 0.08                                                                                                                                                    |
| `discount`                                                                                                                                              | [operations.ComCrmOrderSelfServiceResourceGetOrderItemDiscount](../../models/operations/com-crm-order-self-service-resource-get-order-item-discount.md) | :heavy_minus_sign:                                                                                                                                      | Applied discounton the ordered item                                                                                                                     |                                                                                                                                                         |
| `subTotal`                                                                                                                                              | *number*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | The sub-total of the product before applying the discount. Tax amount is included                                                                       | 1.78                                                                                                                                                    |
| `total`                                                                                                                                                 | *number*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | Order item's total amount                                                                                                                               | 3.4                                                                                                                                                     |
| `priceTerms`                                                                                                                                            | [operations.ComCrmOrderSelfServiceResourceGetOrderPriceTerms](../../models/operations/com-crm-order-self-service-resource-get-order-price-terms.md)     | :heavy_minus_sign:                                                                                                                                      | Applicable when the order item is a Termed or One-Time service. Includes detailed information on the service's pricing terms.                           |                                                                                                                                                         |
| `product`                                                                                                                                               | [operations.ComCrmOrderSelfServiceResourceGetOrderProduct](../../models/operations/com-crm-order-self-service-resource-get-order-product.md)            | :heavy_minus_sign:                                                                                                                                      | Product that was ordered                                                                                                                                |                                                                                                                                                         |
| `taxModel`                                                                                                                                              | [operations.ComCrmOrderSelfServiceResourceGetOrderTaxModel](../../models/operations/com-crm-order-self-service-resource-get-order-tax-model.md)         | :heavy_minus_sign:                                                                                                                                      | N/A                                                                                                                                                     | TAX_INCLUSIVE                                                                                                                                           |
| `devices`                                                                                                                                               | [operations.ComCrmOrderSelfServiceResourceGetOrderDevice](../../models/operations/com-crm-order-self-service-resource-get-order-device.md)[]            | :heavy_minus_sign:                                                                                                                                      | List of strings of device serial numbers                                                                                                                |                                                                                                                                                         |