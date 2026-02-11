# ComCrmOrderSelfServiceResourceGetOrderResponse

OK

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceGetOrderResponse } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourceGetOrderResponse = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  number: "O000001",
  isFavorite: true,
  total: 14.99,
  walletFunds: 1.98,
  amountDue: 13.01,
  currencyCode: "EUR",
  fulfilledBy: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "CRM Nicosia",
    phone: "+6934222321",
    address: {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      addressLine1: "Elia Papakyriakou 21",
      addressLine2: "7 Tower Stars",
      stateProvinceCounty: "Egkomi",
      townCity: "Nicosia",
      postalCode: "2415",
      countryCode: "CYP",
      lat: 35.157115,
      lon: 33.313719,
      googlePlaceId: "ChIJrTLr-GyuEmsRBfy61i59si0",
    },
  },
  address: {
    addressType: "HOME",
    addressName: "My house",
    addressLine1: "17 Baker Str",
    addressLine2: "7 Tower Stars",
    stateProvinceCounty: "Egkomi",
    townCity: "Nicosia",
    postalCode: "12462",
    countryCode: "GRC",
    lat: 12.345,
    lon: 11.452,
    googlePlaceId: "123ewd23rwe23w",
  },
  category: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Normal",
  },
  keyDates: {
    submittedOn: 1592809457,
    completedOn: 1592809457,
    cancelledOn: 1592809457,
    requestedDate: 1649337036,
    startedOn: 1649337036,
    estimatedFulfillment: {
      date: 1592809457,
      duration: 30,
      uot: "MINUTE",
    },
  },
  cancellationReason: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Items out of stock",
  },
  discount: {
    amount: 0.96,
    amountInclTax: 0.98,
  },
  totalDefaultCurrency: 0.97,
  exchangeRate: 0.97,
  defaultCurrencyCode: "EUR",
  preferredBillingDay: {
    dayOfWeek: "MONDAY",
    dayOfMonth: 1,
    monthOfYear: "1",
  },
  items: [
    {
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
      },
      taxModel: "TAX_INCLUSIVE",
      devices: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        },
      ],
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

| Field                                                                                                                                                                                                                           | Type                                                                                                                                                                                                                            | Required                                                                                                                                                                                                                        | Description                                                                                                                                                                                                                     | Example                                                                                                                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                                                            | *string*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | The entity identifier                                                                                                                                                                                                           | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                                            |
| `number`                                                                                                                                                                                                                        | *string*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | Order number                                                                                                                                                                                                                    | O000001                                                                                                                                                                                                                         |
| `supplyMethod`                                                                                                                                                                                                                  | [operations.ComCrmOrderSelfServiceResourceGetOrderSupplyMethod](../../models/operations/com-crm-order-self-service-resource-get-order-supply-method.md)                                                                         | :heavy_minus_sign:                                                                                                                                                                                                              | Defines the order’ supply method                                                                                                                                                                                                |                                                                                                                                                                                                                                 |
| `state`                                                                                                                                                                                                                         | [operations.ComCrmOrderSelfServiceResourceGetOrderState](../../models/operations/com-crm-order-self-service-resource-get-order-state.md)                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | The order’s life cycle state                                                                                                                                                                                                    |                                                                                                                                                                                                                                 |
| `isFavorite`                                                                                                                                                                                                                    | *boolean*                                                                                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                                                              | Shows the contact's favorite Order                                                                                                                                                                                              | true                                                                                                                                                                                                                            |
| `notes`                                                                                                                                                                                                                         | *string*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | The order general notes                                                                                                                                                                                                         |                                                                                                                                                                                                                                 |
| `total`                                                                                                                                                                                                                         | *number*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | Total cost of the Order, i.e the amount that the contact should pay                                                                                                                                                             | 14.99                                                                                                                                                                                                                           |
| `walletFunds`                                                                                                                                                                                                                   | *number*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             | 1.98                                                                                                                                                                                                                            |
| `amountDue`                                                                                                                                                                                                                     | *number*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | Total amount that the contact still hase to pay in order to fully pay off the Order. This implies that contact might already made some payments.                                                                                | 13.01                                                                                                                                                                                                                           |
| `currencyCode`                                                                                                                                                                                                                  | *string*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             | EUR                                                                                                                                                                                                                             |
| `fulfilledBy`                                                                                                                                                                                                                   | [operations.ComCrmOrderSelfServiceResourceGetOrderFulfilledBy](../../models/operations/com-crm-order-self-service-resource-get-order-fulfilled-by.md)                                                                           | :heavy_minus_sign:                                                                                                                                                                                                              | Details about the organisation from where such event was posted                                                                                                                                                                 |                                                                                                                                                                                                                                 |
| `address`                                                                                                                                                                                                                       | [operations.ComCrmOrderSelfServiceResourceGetOrderAddress](../../models/operations/com-crm-order-self-service-resource-get-order-address.md)                                                                                    | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             |                                                                                                                                                                                                                                 |
| `category`                                                                                                                                                                                                                      | [operations.ComCrmOrderSelfServiceResourceGetOrderCategory](../../models/operations/com-crm-order-self-service-resource-get-order-category.md)                                                                                  | :heavy_minus_sign:                                                                                                                                                                                                              | Details about the category                                                                                                                                                                                                      |                                                                                                                                                                                                                                 |
| `keyDates`                                                                                                                                                                                                                      | [operations.KeyDates](../../models/operations/key-dates.md)                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             |                                                                                                                                                                                                                                 |
| `cancellationReason`                                                                                                                                                                                                            | [operations.CancellationReason](../../models/operations/cancellation-reason.md)                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             |                                                                                                                                                                                                                                 |
| `amountToCollect`                                                                                                                                                                                                               | *number*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             |                                                                                                                                                                                                                                 |
| `discount`                                                                                                                                                                                                                      | [operations.ComCrmOrderSelfServiceResourceGetOrderDiscount](../../models/operations/com-crm-order-self-service-resource-get-order-discount.md)                                                                                  | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             |                                                                                                                                                                                                                                 |
| `subTotal`                                                                                                                                                                                                                      | *number*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | Total cost before applying the discount, if any. Tax amount is included                                                                                                                                                         |                                                                                                                                                                                                                                 |
| `netAmount`                                                                                                                                                                                                                     | *number*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             |                                                                                                                                                                                                                                 |
| `taxAmount`                                                                                                                                                                                                                     | *number*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             |                                                                                                                                                                                                                                 |
| `totalDefaultCurrency`                                                                                                                                                                                                          | *number*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | The total in default currency                                                                                                                                                                                                   | 0.97                                                                                                                                                                                                                            |
| `exchangeRate`                                                                                                                                                                                                                  | *number*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | The exchange rate                                                                                                                                                                                                               | 0.97                                                                                                                                                                                                                            |
| `defaultCurrencyCode`                                                                                                                                                                                                           | *string*                                                                                                                                                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | The default currency code                                                                                                                                                                                                       | EUR                                                                                                                                                                                                                             |
| `preferredBillingDay`                                                                                                                                                                                                           | [operations.ComCrmOrderSelfServiceResourceGetOrderPreferredBillingDay](../../models/operations/com-crm-order-self-service-resource-get-order-preferred-billing-day.md)                                                          | :heavy_minus_sign:                                                                                                                                                                                                              | Allows contacts to specify their preferred billing day at the time of ordering. Optional but applicable only when Anniversary billing is enabled and the order includes termed services with billing cycles longer than a week. |                                                                                                                                                                                                                                 |
| `items`                                                                                                                                                                                                                         | [operations.ComCrmOrderSelfServiceResourceGetOrderItem](../../models/operations/com-crm-order-self-service-resource-get-order-item.md)[]                                                                                        | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             |                                                                                                                                                                                                                                 |
| `customFields`                                                                                                                                                                                                                  | [operations.ComCrmOrderSelfServiceResourceGetOrderCustomField](../../models/operations/com-crm-order-self-service-resource-get-order-custom-field.md)[]                                                                         | :heavy_minus_sign:                                                                                                                                                                                                              | N/A                                                                                                                                                                                                                             |                                                                                                                                                                                                                                 |