# ComCrmOrderSelfServiceResourceListOrdersResponse

OK

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceListOrdersResponse } from "crm/models/operations";

let value: ComCrmOrderSelfServiceResourceListOrdersResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      number: "O000001",
      deliveryMethod: "DIRECT_DELIVERY",
      isFavorite: true,
      total: 14.99,
      walletFunds: 1.98,
      amountDue: 13.01,
      currency: "EUR",
      submittedDate: 11599124760,
      fulfilledBy: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "CRM Nicosia",
      },
      discount: {
        amount: 0.96,
        amountInclTax: 0.98,
      },
      netAmount: 9.99,
      taxAmount: 9.99,
      totalDefaultCurrency: 0.97,
      exchangeRate: 0.97,
      defaultCurrencyCode: "EUR",
      stage: {
        id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
        name: "Universal Name",
      },
      preferredBillingDay: {
        dayOfWeek: "MONDAY",
        dayOfMonth: 1,
        monthOfYear: "1",
      },
      customFields: [
        {
          key: "back_office",
          value: "0001-12345",
        },
      ],
      items: [
        {
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
                    url:
                      "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
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
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                              | Type                                                                                                                                               | Required                                                                                                                                           | Description                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                           | [operations.ComCrmOrderSelfServiceResourceListOrdersPaging](../../models/operations/com-crm-order-self-service-resource-list-orders-paging.md)     | :heavy_minus_sign:                                                                                                                                 | N/A                                                                                                                                                |
| `content`                                                                                                                                          | [operations.ComCrmOrderSelfServiceResourceListOrdersContent](../../models/operations/com-crm-order-self-service-resource-list-orders-content.md)[] | :heavy_minus_sign:                                                                                                                                 | N/A                                                                                                                                                |