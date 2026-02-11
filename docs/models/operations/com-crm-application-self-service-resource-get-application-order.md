# ComCrmApplicationSelfServiceResourceGetApplicationOrder

Defines the supported ordering features

## Example Usage

```typescript
import { ComCrmApplicationSelfServiceResourceGetApplicationOrder } from "crmcom/models/operations";

let value: ComCrmApplicationSelfServiceResourceGetApplicationOrder = {
  isSupported: true,
  pickUp: {
    isSupported: true,
    queueId: "b759998f-a452-4019-bda7-457e2e0091a8",
    queueName: "Default queue",
  },
  delivery: {
    isSupported: true,
    queueId: "b759998f-a452-4019-bda7-457e2e0091a8",
    queueName: "Default queue",
  },
  directSale: {
    isSupported: true,
    queueId: "b759998f-a452-4019-bda7-457e2e0091a8",
    queueName: "Default Queue",
  },
  preferredOrganisation: true,
  orderCatalogues: [
    {
      id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
      name: "Universal Name",
    },
  ],
  useWalletFunds: {
    specificFundsAmount: false,
    coverFullBasket: false,
  },
  fulfilmentFlows: {
    fulfilmentFlow: "SINGLE_MERCHANT",
    allowDeliverySelection: true,
  },
  supportProductAdditionalNotes: true,
};
```

## Fields

| Field                                                                                                                                                    | Type                                                                                                                                                     | Required                                                                                                                                                 | Description                                                                                                                                              | Example                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `isSupported`                                                                                                                                            | *boolean*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                       | Defines whether order features should be available                                                                                                       | true                                                                                                                                                     |
| `pickUp`                                                                                                                                                 | [operations.PickUp](../../models/operations/pick-up.md)                                                                                                  | :heavy_minus_sign:                                                                                                                                       | Defines the details for pick up as supply method                                                                                                         | true                                                                                                                                                     |
| `delivery`                                                                                                                                               | [operations.Delivery](../../models/operations/delivery.md)                                                                                               | :heavy_minus_sign:                                                                                                                                       | Defines the details for delivery as supply method                                                                                                        | true                                                                                                                                                     |
| `directSale`                                                                                                                                             | [operations.DirectSale](../../models/operations/direct-sale.md)                                                                                          | :heavy_minus_sign:                                                                                                                                       | Defines the details for direct sale as supply method                                                                                                     | true                                                                                                                                                     |
| `model`                                                                                                                                                  | [operations.Model](../../models/operations/model.md)                                                                                                     | :heavy_minus_sign:                                                                                                                                       | Defines the consumer ordering model                                                                                                                      |                                                                                                                                                          |
| `preferredOrganisation`                                                                                                                                  | *boolean*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                       | Defines whether contact can set preferred organisation for ordering                                                                                      | true                                                                                                                                                     |
| `orderCatalogues`                                                                                                                                        | [operations.OrderCatalogue](../../models/operations/order-catalogue.md)[]                                                                                | :heavy_minus_sign:                                                                                                                                       | Defines a list of order catalogs that should filter available products to order                                                                          |                                                                                                                                                          |
| `useWalletFunds`                                                                                                                                         | [operations.UseWalletFunds](../../models/operations/use-wallet-funds.md)                                                                                 | :heavy_minus_sign:                                                                                                                                       | Defines whether contact can pay for order using wallet funds                                                                                             |                                                                                                                                                          |
| `useAccountFunds`                                                                                                                                        | *boolean*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                       | Allow the contact's account funds to be used for order payments?                                                                                         |                                                                                                                                                          |
| `fulfilmentFlows`                                                                                                                                        | [operations.FulfilmentFlows](../../models/operations/fulfilment-flows.md)                                                                                | :heavy_minus_sign:                                                                                                                                       | Settings that determine the order’s behaviour and how it will be fulfilled by the business and/or the merchants/service provides in the Business Network |                                                                                                                                                          |
| `supportProductAdditionalNotes`                                                                                                                          | *boolean*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                       | Defines if there will be additional notes for each product at the time of ordering                                                                       | true                                                                                                                                                     |