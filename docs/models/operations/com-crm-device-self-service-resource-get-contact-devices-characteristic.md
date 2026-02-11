# ComCrmDeviceSelfServiceResourceGetContactDevicesCharacteristic

## Example Usage

```typescript
import { ComCrmDeviceSelfServiceResourceGetContactDevicesCharacteristic } from "crm/models/operations";

let value: ComCrmDeviceSelfServiceResourceGetContactDevicesCharacteristic = {
  key: "static-ip",
  value: "10.10.01.10",
  label: "Static IP",
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           | Example                                                                               |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `key`                                                                                 | *string*                                                                              | :heavy_check_mark:                                                                    | The characteristic’s key which is unique across the set of configured characteristics | static-ip                                                                             |
| `value`                                                                               | *string*                                                                              | :heavy_check_mark:                                                                    | The actual value of the characteristic                                                | 10.10.01.10                                                                           |
| `label`                                                                               | *string*                                                                              | :heavy_minus_sign:                                                                    | The characteristic's label used for UI purposes                                       | Static IP                                                                             |