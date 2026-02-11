# RewardTiers

Information about the account’s reward tier

## Example Usage

```typescript
import { RewardTiers } from "crmcom/models/operations";

let value: RewardTiers = {
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
              url: "https://asset.crm.com/image/offer/c_scale,w_200/offer.jpg",
            },
          ],
        },
      ],
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                  | Type                                                                                                                                                                   | Required                                                                                                                                                               | Description                                                                                                                                                            | Example                                                                                                                                                                |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                   | *string*                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                     | The entity identifier                                                                                                                                                  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                   |
| `conversionRate`                                                                                                                                                       | *number*                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                     | Defines the conversion rate between real currency and value units                                                                                                      | 1000                                                                                                                                                                   |
| `tiers`                                                                                                                                                                | [operations.ComCrmContactSelfServiceResourceGetSingleWithRewardsTier](../../models/operations/com-crm-contact-self-service-resource-get-single-with-rewards-tier.md)[] | :heavy_minus_sign:                                                                                                                                                     | Defines the supported reward tiers                                                                                                                                     |                                                                                                                                                                        |