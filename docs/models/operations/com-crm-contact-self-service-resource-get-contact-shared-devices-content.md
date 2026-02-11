# ComCrmContactSelfServiceResourceGetContactSharedDevicesContent

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetContactSharedDevicesContent } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceGetContactSharedDevicesContent = {
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
  communityOwner: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "Universal Name",
    code: "4134213343214141",
  },
  device: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    serialNumber: "STB123456",
    customFields: [
      {
        key: "back_office",
        value: "0001-12345",
      },
    ],
  },
};
```

## Fields

| Field                                                                                                                                                                                           | Type                                                                                                                                                                                            | Required                                                                                                                                                                                        | Description                                                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `product`                                                                                                                                                                                       | [operations.ComCrmContactSelfServiceResourceGetContactSharedDevicesProduct](../../models/operations/com-crm-contact-self-service-resource-get-contact-shared-devices-product.md)                | :heavy_minus_sign:                                                                                                                                                                              | N/A                                                                                                                                                                                             |
| `communityOwner`                                                                                                                                                                                | [operations.ComCrmContactSelfServiceResourceGetContactSharedDevicesCommunityOwner](../../models/operations/com-crm-contact-self-service-resource-get-contact-shared-devices-community-owner.md) | :heavy_minus_sign:                                                                                                                                                                              | N/A                                                                                                                                                                                             |
| `device`                                                                                                                                                                                        | [operations.ComCrmContactSelfServiceResourceGetContactSharedDevicesDevice](../../models/operations/com-crm-contact-self-service-resource-get-contact-shared-devices-device.md)                  | :heavy_minus_sign:                                                                                                                                                                              | N/A                                                                                                                                                                                             |