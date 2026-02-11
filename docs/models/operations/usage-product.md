# UsageProduct

The usage product consumed. Can either be a usage service or a non-traceable physical good

## Example Usage

```typescript
import { UsageProduct } from "crm/models/operations";

let value: UsageProduct = {
  id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
  name: "Universal Name",
  sku: "S0001",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `id`                                 | *string*                             | :heavy_minus_sign:                   | The entity identifier                | e283a863-18e1-7cae-48c4-7433bf28cf97 |
| `name`                               | *string*                             | :heavy_minus_sign:                   | The entity name                      | Universal Name                       |
| `sku`                                | *string*                             | :heavy_minus_sign:                   | The entity sku                       | S0001                                |