# OrderCatalogue

## Example Usage

```typescript
import { OrderCatalogue } from "crm/models/operations";

let value: OrderCatalogue = {
  id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
  name: "Universal Name",
};
```

## Fields

| Field                                                                                                          | Type                                                                                                           | Required                                                                                                       | Description                                                                                                    | Example                                                                                                        |
| -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                           | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | The entity identifier                                                                                          | 34b059a3-2aa7-b2c2-4191-a966168e97d7                                                                           |
| `name`                                                                                                         | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | The entity name                                                                                                | Universal Name                                                                                                 |
| `isPricingTable`                                                                                               | *boolean*                                                                                                      | :heavy_minus_sign:                                                                                             | Determines whether the order’s catalogue set up will be presented as a pricing table in front-end apps or not. |                                                                                                                |