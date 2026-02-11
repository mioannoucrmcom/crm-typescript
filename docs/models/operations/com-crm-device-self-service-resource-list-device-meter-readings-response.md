# ComCrmDeviceSelfServiceResourceListDeviceMeterReadingsResponse

OK

## Example Usage

```typescript
import { ComCrmDeviceSelfServiceResourceListDeviceMeterReadingsResponse } from "crmcom/models/operations";

let value: ComCrmDeviceSelfServiceResourceListDeviceMeterReadingsResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "88299a0d-8e17-264a-104d-7d218f5f9a0d",
      reading: 120.99,
      date: {
        from: 1683547447,
        to: 1683547447,
      },
      submittedBy: {
        id: "da8aaf6a-ac3e-ee44-4760-a3b4084b15f4",
        type: "CONTACT",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                            | Type                                                                                                                                                                             | Required                                                                                                                                                                         | Description                                                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                         | [operations.ComCrmDeviceSelfServiceResourceListDeviceMeterReadingsPaging](../../models/operations/com-crm-device-self-service-resource-list-device-meter-readings-paging.md)     | :heavy_minus_sign:                                                                                                                                                               | N/A                                                                                                                                                                              |
| `content`                                                                                                                                                                        | [operations.ComCrmDeviceSelfServiceResourceListDeviceMeterReadingsContent](../../models/operations/com-crm-device-self-service-resource-list-device-meter-readings-content.md)[] | :heavy_minus_sign:                                                                                                                                                               | N/A                                                                                                                                                                              |