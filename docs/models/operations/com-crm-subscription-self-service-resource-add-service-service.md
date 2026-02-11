# ComCrmSubscriptionSelfServiceResourceAddServiceService

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceAddServiceService } from "crmcom/models/operations";

let value: ComCrmSubscriptionSelfServiceResourceAddServiceService = {
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
};
```

## Fields

| Field                                                                                                                                                                | Type                                                                                                                                                                 | Required                                                                                                                                                             | Description                                                                                                                                                          | Example                                                                                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `productId`                                                                                                                                                          | *string*                                                                                                                                                             | :heavy_check_mark:                                                                                                                                                   | The new service product identifier. The product must either be a termed service or a one-time service                                                                | 4dc0809f-ed91-4b68-b912-5bd6064d901e                                                                                                                                 |
| `priceTermsId`                                                                                                                                                       | *string*                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                   | The service's price terms                                                                                                                                            | 1                                                                                                                                                                    |
| `quantity`                                                                                                                                                           | *number*                                                                                                                                                             | :heavy_minus_sign:                                                                                                                                                   | Service quantity. If not specified, then it defaults to 1                                                                                                            | 5                                                                                                                                                                    |
| `components`                                                                                                                                                         | [operations.ComCrmSubscriptionSelfServiceResourceAddServiceComponent](../../models/operations/com-crm-subscription-self-service-resource-add-service-component.md)[] | :heavy_minus_sign:                                                                                                                                                   | List of component services. Applicable only when the service to be added is a flexible bundle                                                                        |                                                                                                                                                                      |
| `devices`                                                                                                                                                            | [operations.ComCrmSubscriptionSelfServiceResourceAddServiceDevice](../../models/operations/com-crm-subscription-self-service-resource-add-service-device.md)[]       | :heavy_minus_sign:                                                                                                                                                   | List of device to which the new service can be enabled on                                                                                                            |                                                                                                                                                                      |