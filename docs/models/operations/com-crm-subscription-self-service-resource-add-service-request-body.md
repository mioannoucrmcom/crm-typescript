# ComCrmSubscriptionSelfServiceResourceAddServiceRequestBody

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceAddServiceRequestBody } from "crm/models/operations";

let value: ComCrmSubscriptionSelfServiceResourceAddServiceRequestBody = {
  scheduledDate: 1621236949,
  pass: {
    code: "SLHY678993109PWE",
    pin: "1245",
  },
  services: [
    {
      productId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
      priceTermsId: "1",
      quantity: 5,
      components: [
        {
          productId: "2dc0809f-ed91-4b68-b912-5bd6064d901e",
          priceTermsId: "32c0809f-ed91-4b68-b912-5bd6064d901e",
        },
      ],
      devices: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        },
      ],
    },
  ],
  paymentMethodId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
  paymentMethodType: "CARD",
};
```

## Fields

| Field                                                                                                                                                                                | Type                                                                                                                                                                                 | Required                                                                                                                                                                             | Description                                                                                                                                                                          | Example                                                                                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `scheduledDate`                                                                                                                                                                      | *number*                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                   | Schedules the addition of the service. The scheduled dat emust be after the current date                                                                                             | 1621236949                                                                                                                                                                           |
| `pass`                                                                                                                                                                               | [operations.ComCrmSubscriptionSelfServiceResourceAddServicePass](../../models/operations/com-crm-subscription-self-service-resource-add-service-pass.md)                             | :heavy_minus_sign:                                                                                                                                                                   | Unlocks a promotion through a (promotion) pass by providing the pass code                                                                                                            |                                                                                                                                                                                      |
| `services`                                                                                                                                                                           | [operations.ComCrmSubscriptionSelfServiceResourceAddServiceService](../../models/operations/com-crm-subscription-self-service-resource-add-service-service.md)[]                     | :heavy_minus_sign:                                                                                                                                                                   | A list of services to be added                                                                                                                                                       |                                                                                                                                                                                      |
| `paymentMethodId`                                                                                                                                                                    | *string*                                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                                   | One of the contact's payment methods that will be used for automatically paying off the subscription. If not specified, then the primary payment method will be used (if any)        | 4dc0809f-ed91-4b68-b912-5bd6064d901e                                                                                                                                                 |
| `paymentMethodType`                                                                                                                                                                  | [operations.ComCrmSubscriptionSelfServiceResourceAddServicePaymentMethodType](../../models/operations/com-crm-subscription-self-service-resource-add-service-payment-method-type.md) | :heavy_minus_sign:                                                                                                                                                                   | The payment method’s type                                                                                                                                                            | CARD                                                                                                                                                                                 |