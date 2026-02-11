# PickUp

Defines the details for pick up as supply method

## Example Usage

```typescript
import { PickUp } from "crm/models/operations";

let value: PickUp = {
  isSupported: true,
  queueId: "b759998f-a452-4019-bda7-457e2e0091a8",
  queueName: "Default queue",
};
```

## Fields

| Field                                            | Type                                             | Required                                         | Description                                      | Example                                          |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| `isSupported`                                    | *boolean*                                        | :heavy_minus_sign:                               | Is pick-up supply method available?              | true                                             |
| `queueId`                                        | *string*                                         | :heavy_minus_sign:                               | Order queue identifier for pick-up supply method | b759998f-a452-4019-bda7-457e2e0091a8             |
| `queueName`                                      | *string*                                         | :heavy_minus_sign:                               | Order queue name for pick-up supply method       | Default queue                                    |