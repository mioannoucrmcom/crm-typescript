# EnabledService

## Example Usage

```typescript
import { EnabledService } from "crmcom/models/operations";

let value: EnabledService = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  lifeCycleState: "EFFECTIVE",
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
  relatedTermedService: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    product: {
      id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
      name: "Universal Name",
      sku: "S0001",
    },
  },
};
```

## Fields

| Field                                                                                                                                                                             | Type                                                                                                                                                                              | Required                                                                                                                                                                          | Description                                                                                                                                                                       | Example                                                                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                              | *string*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The entity identifier                                                                                                                                                             | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                              |
| `lifeCycleState`                                                                                                                                                                  | [operations.ComCrmDeviceSelfServiceResourceGetContactDevicesLifeCycleState](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-life-cycle-state.md) | :heavy_minus_sign:                                                                                                                                                                | Subscription Services State                                                                                                                                                       | EFFECTIVE                                                                                                                                                                         |
| `product`                                                                                                                                                                         | [operations.EnabledServiceProduct](../../models/operations/enabled-service-product.md)                                                                                            | :heavy_minus_sign:                                                                                                                                                                | Details about a product related to a device                                                                                                                                       |                                                                                                                                                                                   |
| `relatedTermedService`                                                                                                                                                            | [operations.RelatedTermedService](../../models/operations/related-termed-service.md)                                                                                              | :heavy_minus_sign:                                                                                                                                                                | Applicable only when the device is enabled on a one-time service which extends a termed service                                                                                   |                                                                                                                                                                                   |