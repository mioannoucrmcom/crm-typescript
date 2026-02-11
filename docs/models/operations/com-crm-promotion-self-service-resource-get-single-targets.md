# ComCrmPromotionSelfServiceResourceGetSingleTargets

The Promotion’s target conditions i.e. the required conditions for the contact to get the discount.

## Example Usage

```typescript
import { ComCrmPromotionSelfServiceResourceGetSingleTargets } from "crmcom/models/operations";

let value: ComCrmPromotionSelfServiceResourceGetSingleTargets = {
  contact: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Universal Name",
  },
  segments: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "VIP contacts",
      description: "The VIP contacts",
      size: 10,
    },
  ],
  organisations: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      name: "Good Burgers",
      type: "MERCHANT",
    },
  ],
  timings: {
    fixedPeriod: {
      startDate: 1648067185,
      endDate: 1648067185,
    },
    availability: null,
  },
};
```

## Fields

| Field                                                                                                                                                              | Type                                                                                                                                                               | Required                                                                                                                                                           | Description                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `contact`                                                                                                                                                          | [operations.ComCrmPromotionSelfServiceResourceGetSingleContact](../../models/operations/com-crm-promotion-self-service-resource-get-single-contact.md)             | :heavy_minus_sign:                                                                                                                                                 | The contact for which the Promotion is applied. Either a Contact or a Segment can be specified in a Promotion                                                      |
| `segments`                                                                                                                                                         | [operations.Segment](../../models/operations/segment.md)[]                                                                                                         | :heavy_minus_sign:                                                                                                                                                 | Either Segments or a specific Contact can be specified per Promotion                                                                                               |
| `organisations`                                                                                                                                                    | [operations.ComCrmPromotionSelfServiceResourceGetSingleOrganisation](../../models/operations/com-crm-promotion-self-service-resource-get-single-organisation.md)[] | :heavy_minus_sign:                                                                                                                                                 | Promotion Location Conditions                                                                                                                                      |
| `timings`                                                                                                                                                          | [operations.Timings](../../models/operations/timings.md)                                                                                                           | :heavy_minus_sign:                                                                                                                                                 | Promotion timings                                                                                                                                                  |