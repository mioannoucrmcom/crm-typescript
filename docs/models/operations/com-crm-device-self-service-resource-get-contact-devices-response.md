# ComCrmDeviceSelfServiceResourceGetContactDevicesResponse

OK

## Example Usage

```typescript
import { ComCrmDeviceSelfServiceResourceGetContactDevicesResponse } from "crm/models/operations";

let value: ComCrmDeviceSelfServiceResourceGetContactDevicesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
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
    },
  ],
};
```

## Fields

| Field                                                                                                                                                               | Type                                                                                                                                                                | Required                                                                                                                                                            | Description                                                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                            | [operations.ComCrmDeviceSelfServiceResourceGetContactDevicesPaging](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-paging.md)     | :heavy_minus_sign:                                                                                                                                                  | N/A                                                                                                                                                                 |
| `content`                                                                                                                                                           | [operations.ComCrmDeviceSelfServiceResourceGetContactDevicesContent](../../models/operations/com-crm-device-self-service-resource-get-contact-devices-content.md)[] | :heavy_minus_sign:                                                                                                                                                  | N/A                                                                                                                                                                 |