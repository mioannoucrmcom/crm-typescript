# ComCrmContactSelfServiceResourceGetContactRelationshipResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetContactRelationshipResponse } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceGetContactRelationshipResponse = {
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
};
```

## Fields

| Field                                                                                                                                                                                        | Type                                                                                                                                                                                         | Required                                                                                                                                                                                     | Description                                                                                                                                                                                  | Example                                                                                                                                                                                      |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                         | *string*                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                           | The contact relationship identifier                                                                                                                                                          | 323a12a6-90e4-fa30-caa4-63e9552ffb10                                                                                                                                                         |
| `relation`                                                                                                                                                                                   | [operations.ComCrmContactSelfServiceResourceGetContactRelationshipRelation](../../models/operations/com-crm-contact-self-service-resource-get-contact-relationship-relation.md)              | :heavy_minus_sign:                                                                                                                                                                           | The community relation that the contact has                                                                                                                                                  |                                                                                                                                                                                              |
| `group`                                                                                                                                                                                      | *string*                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                           | A name that groups together community members                                                                                                                                                | Family                                                                                                                                                                                       |
| `isAdmin`                                                                                                                                                                                    | *boolean*                                                                                                                                                                                    | :heavy_minus_sign:                                                                                                                                                                           | Defines whether the contact member has full permissions. Applicable only for communities of a Contact Company.                                                                               | true                                                                                                                                                                                         |
| `permissions`                                                                                                                                                                                | [operations.ComCrmContactSelfServiceResourceGetContactRelationshipPermission](../../models/operations/com-crm-contact-self-service-resource-get-contact-relationship-permission.md)[]        | :heavy_minus_sign:                                                                                                                                                                           | Defines the (explicit) allowed permissions that the new contact member will have                                                                                                             |                                                                                                                                                                                              |
| `devices`                                                                                                                                                                                    | [operations.ComCrmContactSelfServiceResourceGetContactRelationshipDevice](../../models/operations/com-crm-contact-self-service-resource-get-contact-relationship-device.md)[]                | :heavy_minus_sign:                                                                                                                                                                           | Defines the devices that have been assigned to the community member                                                                                                                          |                                                                                                                                                                                              |
| `contact`                                                                                                                                                                                    | [operations.ComCrmContactSelfServiceResourceGetContactRelationshipContact](../../models/operations/com-crm-contact-self-service-resource-get-contact-relationship-contact.md)                | :heavy_minus_sign:                                                                                                                                                                           | The contact (parent or member in the respective community)                                                                                                                                   |                                                                                                                                                                                              |
| `walletSharing`                                                                                                                                                                              | [operations.ComCrmContactSelfServiceResourceGetContactRelationshipWalletSharing](../../models/operations/com-crm-contact-self-service-resource-get-contact-relationship-wallet-sharing.md)   | :heavy_minus_sign:                                                                                                                                                                           | Defines whether the community person will be able to use/request money from community owner wallet                                                                                           |                                                                                                                                                                                              |
| `usageAllowance`                                                                                                                                                                             | [operations.ComCrmContactSelfServiceResourceGetContactRelationshipUsageAllowance](../../models/operations/com-crm-contact-self-service-resource-get-contact-relationship-usage-allowance.md) | :heavy_minus_sign:                                                                                                                                                                           | Defines the usage allowance                                                                                                                                                                  |                                                                                                                                                                                              |
| `state`                                                                                                                                                                                      | [operations.ComCrmContactSelfServiceResourceGetContactRelationshipState](../../models/operations/com-crm-contact-self-service-resource-get-contact-relationship-state.md)                    | :heavy_minus_sign:                                                                                                                                                                           | The community member’s relation state. A person is considered as a valid community person only after they accept the invitation to join the community.                                       |                                                                                                                                                                                              |
| `termedTransfer`                                                                                                                                                                             | [operations.ComCrmContactSelfServiceResourceGetContactRelationshipTermedTransfer](../../models/operations/com-crm-contact-self-service-resource-get-contact-relationship-termed-transfer.md) | :heavy_minus_sign:                                                                                                                                                                           | The termed transfers set up by the community owner for the community member                                                                                                                  |                                                                                                                                                                                              |