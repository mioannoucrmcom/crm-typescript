# ComCrmSubscriptionSelfServiceResourceListServiceDevicesContent

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListServiceDevicesContent } from "crm/models/operations";

let value: ComCrmSubscriptionSelfServiceResourceListServiceDevicesContent = {
  code: "4345665678888897",
  state: "ENABLED",
  device: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    serialNumber: "STB3332222111",
    eletronicId: "STB3332222111",
    product: {
      id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
      name: "Universal Name",
      sku: "S0001",
    },
  },
};
```

## Fields

| Field                                                                                                                                                                                      | Type                                                                                                                                                                                       | Required                                                                                                                                                                                   | Description                                                                                                                                                                                | Example                                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `code`                                                                                                                                                                                     | *string*                                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                                         | Code that uniquely identifies the distribution of the service to a device. This is a random and unique 16-digit code                                                                       | 4345665678888897                                                                                                                                                                           |
| `state`                                                                                                                                                                                    | [operations.ComCrmSubscriptionSelfServiceResourceListServiceDevicesContentState](../../models/operations/com-crm-subscription-self-service-resource-list-service-devices-content-state.md) | :heavy_minus_sign:                                                                                                                                                                         | Defines whether the service is already enabled on the device or not. If disabled, then the service can be enabled on the related device                                                    | ENABLED                                                                                                                                                                                    |
| `device`                                                                                                                                                                                   | [operations.ComCrmSubscriptionSelfServiceResourceListServiceDevicesDevice](../../models/operations/com-crm-subscription-self-service-resource-list-service-devices-device.md)              | :heavy_minus_sign:                                                                                                                                                                         | The device on which the service is already or could be enabled on. This device is owned or it was rented by the contact                                                                    |                                                                                                                                                                                            |