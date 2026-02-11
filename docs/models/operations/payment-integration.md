# PaymentIntegration

The payment integration type=PURCHASE_PASS

## Example Usage

```typescript
import { PaymentIntegration } from "crm/models/operations";

let value: PaymentIntegration = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  connector: "PLUGIN",
};
```

## Fields

| Field                                                        | Type                                                         | Required                                                     | Description                                                  | Example                                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `id`                                                         | *string*                                                     | :heavy_minus_sign:                                           | The entity identifier                                        | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                         |
| `connector`                                                  | [operations.Connector](../../models/operations/connector.md) | :heavy_minus_sign:                                           | The payment integration connector type                       | PLUGIN                                                       |