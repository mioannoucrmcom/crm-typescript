# DirectSale

Defines the details for direct sale as supply method

## Example Usage

```typescript
import { DirectSale } from "crm/models/operations";

let value: DirectSale = {
  isSupported: true,
  queueId: "b759998f-a452-4019-bda7-457e2e0091a8",
  queueName: "Default Queue",
};
```

## Fields

| Field                                                | Type                                                 | Required                                             | Description                                          | Example                                              |
| ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- |
| `isSupported`                                        | *boolean*                                            | :heavy_minus_sign:                                   | Is direct sale supply method available?              | true                                                 |
| `queueId`                                            | *string*                                             | :heavy_minus_sign:                                   | Order queue identifier for direct-sale supply method | b759998f-a452-4019-bda7-457e2e0091a8                 |
| `queueName`                                          | *string*                                             | :heavy_minus_sign:                                   | Order queue name for direct-sale supply method       | Default Queue                                        |