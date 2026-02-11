# Progress

Details about the next tier progression

## Example Usage

```typescript
import { Progress } from "crm/models/operations";

let value: Progress = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Gold",
  pointsNeeded: 1400,
  collectedBy: 1615996441,
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     | Example                                                                         |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `id`                                                                            | *string*                                                                        | :heavy_minus_sign:                                                              | The entity identifier                                                           | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                            |
| `name`                                                                          | *string*                                                                        | :heavy_minus_sign:                                                              | The next tier name                                                              | Gold                                                                            |
| `pointsNeeded`                                                                  | *number*                                                                        | :heavy_minus_sign:                                                              | Points needed to progress to next tier                                          | 1400                                                                            |
| `collectedBy`                                                                   | *number*                                                                        | :heavy_minus_sign:                                                              | The date up to which points must be collected in order to progress to next tier | 1615996441                                                                      |