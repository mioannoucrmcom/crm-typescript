# ComCrmContactSelfServiceResourceGetContactSharedDevicesResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetContactSharedDevicesResponse } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceGetContactSharedDevicesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
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
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                              | Type                                                                                                                                                                               | Required                                                                                                                                                                           | Description                                                                                                                                                                        |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                           | [operations.ComCrmContactSelfServiceResourceGetContactSharedDevicesPaging](../../models/operations/com-crm-contact-self-service-resource-get-contact-shared-devices-paging.md)     | :heavy_minus_sign:                                                                                                                                                                 | N/A                                                                                                                                                                                |
| `content`                                                                                                                                                                          | [operations.ComCrmContactSelfServiceResourceGetContactSharedDevicesContent](../../models/operations/com-crm-contact-self-service-resource-get-contact-shared-devices-content.md)[] | :heavy_minus_sign:                                                                                                                                                                 | N/A                                                                                                                                                                                |