# ProvisionedDevice

## Example Usage

```typescript
import { ProvisionedDevice } from "crmcom/models/operations";

let value: ProvisionedDevice = {
  device: {
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

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `changeType`                                                                                        | [operations.ProvisionedDeviceChangeType](../../models/operations/provisioned-device-change-type.md) | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `device`                                                                                            | [operations.ProvisionedDeviceDevice](../../models/operations/provisioned-device-device.md)          | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |