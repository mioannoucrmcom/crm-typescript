# ComCrmDeviceSelfServiceResourceGetContactDevicesContent

## Example Usage

```typescript
import { ComCrmDeviceSelfServiceResourceGetContactDevicesContent } from "crmcom/models/operations";

let value: ComCrmDeviceSelfServiceResourceGetContactDevicesContent = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  macAddress: "00:00:5e:00:53:af",
  serialNumber: "2049-3630",
  electronicId: "512f-6a78-4ccbd180bdad",
  registrationToken: "4e11bef819b8ae9af08d",
  registrationDate: 1642758418,
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
  customFields: [
    {
      key: "back_office",
      value: "0001-12345",
    },
  ],
  meterReadings: {
    measurementUnit: {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Gigabytes",
      displayName: "GB",
    },
    type: "ONE_TIME",
  },
  characteristics: [
    {
      key: "static-ip",
      value: "10.10.01.10",
      label: "Static IP",
    },
  ],
  enabledServices: [
    {
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
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                             | Type                                                                                                                                                                              | Required                                                                                                                                                                          | Description                                                                                                                                                                       | Example                                                                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                              | *string*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The entity identifier                                                                                                                                                             | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                              |
| `macAddress`                                                                                                                                                                      | *string*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The device’s MAC address                                                                                                                                                          | 00:00:5e:00:53:af                                                                                                                                                                 |
| `platform`                                                                                                                                                                        | [operations.ComCrmDeviceSelfServiceResourceGetContactDevicesPlatform](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-platform.md)               | :heavy_minus_sign:                                                                                                                                                                | The device’s operation platform                                                                                                                                                   |                                                                                                                                                                                   |
| `serialNumber`                                                                                                                                                                    | *string*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The device’s serial number                                                                                                                                                        | 2049-3630                                                                                                                                                                         |
| `electronicId`                                                                                                                                                                    | *string*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The device electronic id                                                                                                                                                          | 512f-6a78-4ccbd180bdad                                                                                                                                                            |
| `registrationToken`                                                                                                                                                               | *string*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The device’s registration token for push notifications                                                                                                                            | 4e11bef819b8ae9af08d                                                                                                                                                              |
| `registrationDate`                                                                                                                                                                | *number*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                | The date that such device was registered by the contact                                                                                                                           | 1642758418                                                                                                                                                                        |
| `product`                                                                                                                                                                         | [operations.ComCrmDeviceSelfServiceResourceGetContactDevicesProduct](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-product.md)                 | :heavy_minus_sign:                                                                                                                                                                | Details about the product that defines such device                                                                                                                                |                                                                                                                                                                                   |
| `customFields`                                                                                                                                                                    | [operations.ComCrmDeviceSelfServiceResourceGetContactDevicesCustomField](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-custom-field.md)[]      | :heavy_minus_sign:                                                                                                                                                                | N/A                                                                                                                                                                               |                                                                                                                                                                                   |
| `meterReadings`                                                                                                                                                                   | [operations.MeterReadings](../../models/operations/meter-readings.md)                                                                                                             | :heavy_minus_sign:                                                                                                                                                                | Details about the meter readings supported by this device                                                                                                                         |                                                                                                                                                                                   |
| `characteristics`                                                                                                                                                                 | [operations.ComCrmDeviceSelfServiceResourceGetContactDevicesCharacteristic](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-characteristic.md)[] | :heavy_minus_sign:                                                                                                                                                                | The device characteristics (specified per product, product type or device)                                                                                                        |                                                                                                                                                                                   |
| `enabledServices`                                                                                                                                                                 | [operations.EnabledService](../../models/operations/enabled-service.md)[]                                                                                                         | :heavy_minus_sign:                                                                                                                                                                | The enabled services for the device. List of services includes all services of the specified subscription.                                                                        |                                                                                                                                                                                   |