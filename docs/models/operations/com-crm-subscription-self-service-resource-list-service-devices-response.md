# ComCrmSubscriptionSelfServiceResourceListServiceDevicesResponse

OK

## Example Usage

```typescript
import { ComCrmSubscriptionSelfServiceResourceListServiceDevicesResponse } from "crmcom/models/operations";

let value: ComCrmSubscriptionSelfServiceResourceListServiceDevicesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
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
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                             | Type                                                                                                                                                                              | Required                                                                                                                                                                          | Description                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                          | [operations.ComCrmSubscriptionSelfServiceResourceListServiceDevicesPaging](../../models/operations/com-crm-subscription-self-service-resource-list-service-devices-paging.md)     | :heavy_minus_sign:                                                                                                                                                                | N/A                                                                                                                                                                               |
| `content`                                                                                                                                                                         | [operations.ComCrmSubscriptionSelfServiceResourceListServiceDevicesContent](../../models/operations/com-crm-subscription-self-service-resource-list-service-devices-content.md)[] | :heavy_minus_sign:                                                                                                                                                                | N/A                                                                                                                                                                               |