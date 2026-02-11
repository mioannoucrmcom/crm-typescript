# ComCrmOrderSelfServiceResourceListOrdersItem

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceListOrdersItem } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourceListOrdersItem = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  quantity: 2,
  lifeCycleState: "PENDING_DELIVERY",
  product: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    sku: "0123-112",
    name: "Decoder",
    quantity: 2,
    price: 1.7,
    cost: 3.4,
    classification: "TRACEABLE_PHYSICAL_GOOD",
    taxAmount: 0.08,
    costBeforeDiscount: 1.78,
    variantAttributes: [
      {
        key: "size",
        value: "Grande",
        name: "Size",
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
    tags: [
      {
        tagId: "JKGJHFSDJHGDSJHGA",
        name: "Maintenance",
      },
    ],
    priceTerms: {
      billingPeriod: {
        duration: 1,
        uot: "MONTH",
      },
    },
  },
};
```

## Fields

| Field                                                                                                                                                            | Type                                                                                                                                                             | Required                                                                                                                                                         | Description                                                                                                                                                      | Example                                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                             | *string*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | The entity identifier                                                                                                                                            | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                             |
| `quantity`                                                                                                                                                       | *number*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | The quantity of the ordered items                                                                                                                                | 2                                                                                                                                                                |
| `notes`                                                                                                                                                          | *string*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | N/A                                                                                                                                                              |                                                                                                                                                                  |
| `lifeCycleState`                                                                                                                                                 | [operations.ComCrmOrderSelfServiceResourceListOrdersLifeCycleState](../../models/operations/com-crm-order-self-service-resource-list-orders-life-cycle-state.md) | :heavy_minus_sign:                                                                                                                                               | The order item state                                                                                                                                             | PENDING_DELIVERY                                                                                                                                                 |
| `product`                                                                                                                                                        | [operations.ComCrmOrderSelfServiceResourceListOrdersProduct](../../models/operations/com-crm-order-self-service-resource-list-orders-product.md)                 | :heavy_minus_sign:                                                                                                                                               | Details about the ordered product                                                                                                                                |                                                                                                                                                                  |