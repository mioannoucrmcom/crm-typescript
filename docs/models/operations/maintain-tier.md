# MaintainTier

Details on how to maintain the current tier

## Example Usage

```typescript
import { MaintainTier } from "crmcom/models/operations";

let value: MaintainTier = {
  pointsNeeded: 200,
  collectedBy: 1615996441,
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            | Example                                                                                |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `pointsNeeded`                                                                         | *number*                                                                               | :heavy_minus_sign:                                                                     | The number of points needed to maintain current tier                                   | 200                                                                                    |
| `collectedBy`                                                                          | *number*                                                                               | :heavy_minus_sign:                                                                     | The date up to which points must be collected by in order to maintain the current tier | 1615996441                                                                             |