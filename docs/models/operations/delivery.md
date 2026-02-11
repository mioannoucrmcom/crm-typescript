# Delivery

Defines the details for delivery as supply method

## Example Usage

```typescript
import { Delivery } from "crmcom/models/operations";

let value: Delivery = {
  isSupported: true,
  queueId: "b759998f-a452-4019-bda7-457e2e0091a8",
  queueName: "Default queue",
};
```

## Fields

| Field                                             | Type                                              | Required                                          | Description                                       | Example                                           |
| ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- |
| `isSupported`                                     | *boolean*                                         | :heavy_minus_sign:                                | Is delivery supply method available?              | true                                              |
| `queueId`                                         | *string*                                          | :heavy_minus_sign:                                | Order queue identifier for delivery supply method | b759998f-a452-4019-bda7-457e2e0091a8              |
| `queueName`                                       | *string*                                          | :heavy_minus_sign:                                | Order queue name for delivery supply method       | Default queue                                     |