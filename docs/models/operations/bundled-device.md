# BundledDevice

Applicable when the service was added as part of a bundled device

## Example Usage

```typescript
import { BundledDevice } from "crm/models/operations";

let value: BundledDevice = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  serialNumber: "STB3332222111",
  product: {
    id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
    name: "Universal Name",
    sku: "S0001",
  },
};
```

## Fields

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          | Example                                                                              |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `id`                                                                                 | *string*                                                                             | :heavy_minus_sign:                                                                   | The entity identifier                                                                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                 |
| `serialNumber`                                                                       | *string*                                                                             | :heavy_minus_sign:                                                                   | Bundle device serial number                                                          | STB3332222111                                                                        |
| `product`                                                                            | [operations.BundledDeviceProduct](../../models/operations/bundled-device-product.md) | :heavy_minus_sign:                                                                   | Bundle device product                                                                |                                                                                      |