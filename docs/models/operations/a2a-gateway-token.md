# A2aGatewayToken

## Example Usage

```typescript
import { A2aGatewayToken } from "crm/models/operations";

let value: A2aGatewayToken = {
  gateway: "JCC",
  token: "Xt5EWLLDS7FJjR1c",
  integration: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Universal Name",
  },
};
```

## Fields

| Field                                                                   | Type                                                                    | Required                                                                | Description                                                             | Example                                                                 |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `gateway`                                                               | *string*                                                                | :heavy_minus_sign:                                                      | Defines the gateway that issued such token                              | JCC                                                                     |
| `token`                                                                 | *string*                                                                | :heavy_minus_sign:                                                      | The card related token                                                  | Xt5EWLLDS7FJjR1c                                                        |
| `integration`                                                           | [operations.A2aIntegration](../../models/operations/a2a-integration.md) | :heavy_minus_sign:                                                      | The gateway integration                                                 |                                                                         |