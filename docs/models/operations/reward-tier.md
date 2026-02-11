# RewardTier

Information about the account’s reward tier

## Example Usage

```typescript
import { RewardTier } from "crmcom/models/operations";

let value: RewardTier = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Red",
  colour: "#d4af37",
  achievedDate: 1615996441,
  periodValueUnits: 2000,
  lifetimeValueUnits: 12543,
  maintainTier: {
    pointsNeeded: 200,
    collectedBy: 1615996441,
  },
  progress: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    name: "Gold",
    pointsNeeded: 1400,
    collectedBy: 1615996441,
  },
  creatives: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      width: 2159,
      height: 3075,
      format: "jpg",
      url: "https://assets.crm.com/image/offer.jpg",
      publicId: "crm-com/image",
      media: [
        {
          width: 200,
          height: 300,
          url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      | Example                                                                                          |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `id`                                                                                             | *string*                                                                                         | :heavy_minus_sign:                                                                               | The entity identifier                                                                            | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                             |
| `name`                                                                                           | *string*                                                                                         | :heavy_minus_sign:                                                                               | The reward tier name                                                                             | Red                                                                                              |
| `colour`                                                                                         | *string*                                                                                         | :heavy_minus_sign:                                                                               | The tier (marketing) colour                                                                      | #d4af37                                                                                          |
| `achievedDate`                                                                                   | *number*                                                                                         | :heavy_minus_sign:                                                                               | The date that the current tier was reached                                                       | 1615996441                                                                                       |
| `periodValueUnits`                                                                               | *number*                                                                                         | :heavy_minus_sign:                                                                               | Points collected during the period                                                               | 2000                                                                                             |
| `lifetimeValueUnits`                                                                             | *number*                                                                                         | :heavy_minus_sign:                                                                               | Total Lifetime Points                                                                            | 12543                                                                                            |
| `maintainTier`                                                                                   | [operations.MaintainTier](../../models/operations/maintain-tier.md)                              | :heavy_minus_sign:                                                                               | Details on how to maintain the current tier                                                      |                                                                                                  |
| `progress`                                                                                       | [operations.Progress](../../models/operations/progress.md)                                       | :heavy_minus_sign:                                                                               | Details about the next tier progression                                                          |                                                                                                  |
| `creatives`                                                                                      | [operations.RewardTierCreative](../../models/operations/reward-tier-creative.md)[]               | :heavy_minus_sign:                                                                               | Creatives images for marketing includes the primary image and scaled versions to create a srcset |                                                                                                  |