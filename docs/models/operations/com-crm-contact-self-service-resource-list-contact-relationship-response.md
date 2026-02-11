# ComCrmContactSelfServiceResourceListContactRelationshipResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceListContactRelationshipResponse } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceListContactRelationshipResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
      id: "323a12a6-90e4-fa30-caa4-63e9552ffb10",
      relation: {
        id: "9aabba32-82e3-441f-969a-103d81e2f91f",
        name: "Employees",
      },
      group: "Family",
      isAdmin: true,
      devices: [
        {
          id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
          serialNumber: "STB123456",
          customFields: [
            {
              key: "back_office",
              value: "0001-12345",
            },
          ],
        },
      ],
      contact: {
        id: "19e631ac-4123-1099-d207-2a70fb126186",
        firstName: "John",
        lastName: "Smith",
        phone: {
          countryCode: "CYP",
          number: "744444121",
        },
        email: "johndoe@crm.com",
        wallet: {
          id: "dccc7b0d-0626-dd0e-88e3-67a1cc0bf610",
        },
      },
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
      termedTransfer: {
        isEnabled: true,
        amount: 100,
        currencyCode: "EUR",
        commercePool: {
          id: "dc01f65b-a482-48f1-9fda-c163df72f28f",
          name: "Redeem Anywhere",
        },
        schedule: {
          frequency: "MONTHLY",
          dayOfWeek: "MONDAY",
          dayOfMonth: 15,
        },
      },
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                             | Type                                                                                                                                                                              | Required                                                                                                                                                                          | Description                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                                          | [operations.ComCrmContactSelfServiceResourceListContactRelationshipPaging](../../models/operations/com-crm-contact-self-service-resource-list-contact-relationship-paging.md)     | :heavy_minus_sign:                                                                                                                                                                | N/A                                                                                                                                                                               |
| `content`                                                                                                                                                                         | [operations.ComCrmContactSelfServiceResourceListContactRelationshipContent](../../models/operations/com-crm-contact-self-service-resource-list-contact-relationship-content.md)[] | :heavy_minus_sign:                                                                                                                                                                | N/A                                                                                                                                                                               |