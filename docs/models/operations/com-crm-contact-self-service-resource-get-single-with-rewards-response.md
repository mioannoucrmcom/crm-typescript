# ComCrmContactSelfServiceResourceGetSingleWithRewardsResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetSingleWithRewardsResponse } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceGetSingleWithRewardsResponse = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  rewardSchemes: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "CRMdotCOM Scheme",
      signedUpOn: 1583846865,
      emailAddress: "johndoe@crm.com",
    },
  ],
  signUpDate: 1583846865,
  spendBlocked: {
    date: 1583846865,
    status: true,
  },
  rewardTier: {
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
  },
  rewardTiers: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    conversionRate: 1000,
    tiers: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        name: "Gold",
        description: "Gold Customers",
        color: "#d4af37",
        valueUnits: 150000,
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
                url:
                  "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
              },
            ],
          },
        ],
      },
    ],
  },
};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            | Example                                                                |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `id`                                                                   | *string*                                                               | :heavy_minus_sign:                                                     | The entity identifier                                                  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                   |
| `rewardSchemes`                                                        | [operations.RewardScheme](../../models/operations/reward-scheme.md)[]  | :heavy_minus_sign:                                                     | Details about the already signed up reward schemes                     |                                                                        |
| `signUpDate`                                                           | *number*                                                               | :heavy_minus_sign:                                                     | The date when the contact was signed up to a scheme for the first time | 1583846865                                                             |
| `spendBlocked`                                                         | [operations.SpendBlocked](../../models/operations/spend-blocked.md)    | :heavy_minus_sign:                                                     | Details about whether the contact can spend or not                     |                                                                        |
| `rewardTier`                                                           | [operations.RewardTier](../../models/operations/reward-tier.md)        | :heavy_minus_sign:                                                     | Information about the account’s reward tier                            |                                                                        |
| `rewardTiers`                                                          | [operations.RewardTiers](../../models/operations/reward-tiers.md)      | :heavy_minus_sign:                                                     | Information about the account’s reward tier                            |                                                                        |