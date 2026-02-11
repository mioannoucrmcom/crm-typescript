# ComCrmDeviceSelfServiceResourceUpdateDeviceRequestBody

## Example Usage

```typescript
import { ComCrmDeviceSelfServiceResourceUpdateDeviceRequestBody } from "crm/models/operations";

let value: ComCrmDeviceSelfServiceResourceUpdateDeviceRequestBody = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  customFields: [
    {
      key: "back_office",
      value: "0001-12345",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                             | Type                                                                                                                                                              | Required                                                                                                                                                          | Description                                                                                                                                                       | Example                                                                                                                                                           |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                              | *string*                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                | The entity identifier that will be created                                                                                                                        | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                              |
| `customFields`                                                                                                                                                    | [operations.ComCrmDeviceSelfServiceResourceUpdateDeviceCustomField](../../models/operations/com-crm-device-self-service-resource-update-device-custom-field.md)[] | :heavy_minus_sign:                                                                                                                                                | A list of custom fields whose values can be set when creating or updating entities                                                                                |                                                                                                                                                                   |