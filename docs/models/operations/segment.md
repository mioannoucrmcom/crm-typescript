# Segment

## Example Usage

```typescript
import { Segment } from "crmcom/models/operations";

let value: Segment = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "VIP contacts",
  description: "The VIP contacts",
  size: 10,
};
```

## Fields

| Field                                             | Type                                              | Required                                          | Description                                       | Example                                           |
| ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- |
| `id`                                              | *string*                                          | :heavy_minus_sign:                                | The entity identifier                             | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0              |
| `name`                                            | *string*                                          | :heavy_minus_sign:                                | The name of the Segment                           | VIP contacts                                      |
| `description`                                     | *string*                                          | :heavy_minus_sign:                                | The description of the Segment                    | The VIP contacts                                  |
| `size`                                            | *number*                                          | :heavy_minus_sign:                                | The number of contacts retrieved from the Segment | 10                                                |