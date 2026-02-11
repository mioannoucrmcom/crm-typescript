# ComCrmContactSelfServiceResourceGetCommunitiesContent

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetCommunitiesContent } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceGetCommunitiesContent = {
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
};
```

## Fields

| Field                                                                                                                                                                       | Type                                                                                                                                                                        | Required                                                                                                                                                                    | Description                                                                                                                                                                 | Example                                                                                                                                                                     |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `communityOwner`                                                                                                                                                            | [operations.ComCrmContactSelfServiceResourceGetCommunitiesCommunityOwner](../../models/operations/com-crm-contact-self-service-resource-get-communities-community-owner.md) | :heavy_minus_sign:                                                                                                                                                          | The contact that is owner of the community that the related contact is a member to                                                                                          |                                                                                                                                                                             |
| `relation`                                                                                                                                                                  | [operations.ComCrmContactSelfServiceResourceGetCommunitiesRelation](../../models/operations/com-crm-contact-self-service-resource-get-communities-relation.md)              | :heavy_minus_sign:                                                                                                                                                          | The community relation that the contact has                                                                                                                                 |                                                                                                                                                                             |
| `isAdmin`                                                                                                                                                                   | *boolean*                                                                                                                                                                   | :heavy_minus_sign:                                                                                                                                                          | Defines whether the contact member will have full permissions                                                                                                               | true                                                                                                                                                                        |
| `permissions`                                                                                                                                                               | [operations.ComCrmContactSelfServiceResourceGetCommunitiesPermission](../../models/operations/com-crm-contact-self-service-resource-get-communities-permission.md)[]        | :heavy_minus_sign:                                                                                                                                                          | Defines the (explicit) allowed permissions that the new contact member will have                                                                                            |                                                                                                                                                                             |
| `walletSharing`                                                                                                                                                             | [operations.ComCrmContactSelfServiceResourceGetCommunitiesWalletSharing](../../models/operations/com-crm-contact-self-service-resource-get-communities-wallet-sharing.md)   | :heavy_minus_sign:                                                                                                                                                          | Defines whether the community person will be able to use/request money from community owner wallet                                                                          |                                                                                                                                                                             |
| `usageAllowance`                                                                                                                                                            | [operations.ComCrmContactSelfServiceResourceGetCommunitiesUsageAllowance](../../models/operations/com-crm-contact-self-service-resource-get-communities-usage-allowance.md) | :heavy_minus_sign:                                                                                                                                                          | Defines the usage allowance                                                                                                                                                 |                                                                                                                                                                             |
| `state`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceGetCommunitiesState](../../models/operations/com-crm-contact-self-service-resource-get-communities-state.md)                    | :heavy_minus_sign:                                                                                                                                                          | The community people person's relation state. A person is considered as a valid community person only after they accept the invitation to join the community.               |                                                                                                                                                                             |
| `group`                                                                                                                                                                     | *string*                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                          | A name that groups together community members                                                                                                                               | Family                                                                                                                                                                      |