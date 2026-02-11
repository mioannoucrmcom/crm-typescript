# ComCrmContactSelfServiceResourceGetCommunitiesResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetCommunitiesResponse } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceGetCommunitiesResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      communityOwner: {
        id: "b22e6e44-2c3c-af17-27ac-bacad6cf7181",
        firstName: "John",
        lastName: "Doe",
        wallet: {
          id: "dccc7b0d-0626-dd0e-88e3-67a1cc0bf610",
        },
        companyName: "CRM",
      },
      relation: {
        id: "9aabba32-82e3-441f-969a-103d81e2f91f",
        name: "Employees",
      },
      isAdmin: true,
      walletSharing: {
        isEnabled: true,
        commercePools: [
          {
            id: "dc01f65b-a482-48f1-9fda-c163df72f28f",
            name: "Redeem Anywhere",
            description: "Ability to redeem on any organisation/day/product",
          },
        ],
        method: "AUTO",
        maxAmount: 50,
        remainingAmount: 1.99,
      },
      usageAllowance: {
        accumulatedAllowance: {
          currency: "EUR",
        },
        productsAllowance: [
          {
            id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
            currency: "EUR",
            itemType: "PRODUCT",
            itemId: "4dc0809f-ed91-4b68-b912-5bd6064d901e",
            name: "Bronze",
            measurementUnit: {
              name: "Gigabytes",
              displayName: "GB",
            },
          },
        ],
        organisations: [
          {
            id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
            name: "Universal Name",
          },
        ],
      },
      group: "Family",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                          | Type                                                                                                                                                           | Required                                                                                                                                                       | Description                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                       | [operations.ComCrmContactSelfServiceResourceGetCommunitiesPaging](../../models/operations/com-crm-contact-self-service-resource-get-communities-paging.md)     | :heavy_minus_sign:                                                                                                                                             | N/A                                                                                                                                                            |
| `content`                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceGetCommunitiesContent](../../models/operations/com-crm-contact-self-service-resource-get-communities-content.md)[] | :heavy_minus_sign:                                                                                                                                             | N/A                                                                                                                                                            |