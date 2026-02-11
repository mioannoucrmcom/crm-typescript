# MeterReadings

Details about the meter readings supported by this device

## Example Usage

```typescript
import { MeterReadings } from "crm/models/operations";

let value: MeterReadings = {
  measurementUnit: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "Gigabytes",
    displayName: "GB",
  },
  type: "ONE_TIME",
};
```

## Fields

| Field                                                                                                                                                                              | Type                                                                                                                                                                               | Required                                                                                                                                                                           | Description                                                                                                                                                                        | Example                                                                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `measurementUnit`                                                                                                                                                                  | [operations.ComCrmDeviceSelfServiceResourceGetContactDevicesMeasurementUnit](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-measurement-unit.md) | :heavy_minus_sign:                                                                                                                                                                 | The device's meter reading unit of measurement (as specified on the related product)                                                                                               |                                                                                                                                                                                    |
| `type`                                                                                                                                                                             | [operations.ComCrmDeviceSelfServiceResourceGetContactDevicesType](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-type.md)                        | :heavy_minus_sign:                                                                                                                                                                 | The device meter reading type (one-time or cumulative)                                                                                                                             | ONE_TIME                                                                                                                                                                           |