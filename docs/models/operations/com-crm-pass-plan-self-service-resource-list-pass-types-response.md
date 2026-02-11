# ComCrmPassPlanSelfServiceResourceListPassTypesResponse

OK

## Example Usage

```typescript
import { ComCrmPassPlanSelfServiceResourceListPassTypesResponse } from "crm/models/operations";

let value: ComCrmPassPlanSelfServiceResourceListPassTypesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      state: "ACTIVE",
      name: "Xmas Gift Cards",
      description: "Gift Cards for Christmas",
      classification: "GIFT",
      promotionPasses: {
        promotionId: "e2ade504-9b90-92be-0adb-3258475ff695",
        rewardOfferId: "e2ade504-9b90-92be-0adb-3258475ff695",
        name: "50% Birthday Offer",
        maximumUsage: 1,
      },
      validity: {
        type: "ALWAYS",
        period: 1,
        uot: "MONTHS",
        fixedDate: 1591703675,
      },
      value: {
        type: "FIXED",
        fixedAmount: 100,
        minimum: 10,
        maximum: 50,
        currencyCode: "EUR",
      },
      printed: true,
      codeFormat: {
        type: "ALPHANUMERIC",
        prefix: "CRM",
        suffix: "2020",
        length: 10,
        pinRequired: true,
        singleCode: "\"123456\"",
      },
      creditWalletBalance: "COMMERCE",
      commercePool: {
        id: "dc01f65b-a482-48f1-9fda-c163df72f28f",
        name: "Redeem Anywhere",
        description: "Ability to redeem on any organisation/day/product",
      },
      numberOfPasses: 100,
      customFields: [
        {
          key: "back_office",
          value: "0001-12345",
        },
      ],
      currencyCode: "EUR",
      product: {
        id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
        name: "Universal Name",
        sku: "S0001",
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                            | Type                                                                                                                                                             | Required                                                                                                                                                         | Description                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                         | [operations.ComCrmPassPlanSelfServiceResourceListPassTypesPaging](../../models/operations/com-crm-pass-plan-self-service-resource-list-pass-types-paging.md)     | :heavy_minus_sign:                                                                                                                                               | N/A                                                                                                                                                              |
| `content`                                                                                                                                                        | [operations.ComCrmPassPlanSelfServiceResourceListPassTypesContent](../../models/operations/com-crm-pass-plan-self-service-resource-list-pass-types-content.md)[] | :heavy_minus_sign:                                                                                                                                               | N/A                                                                                                                                                              |