# ComCrmContactSelfServiceResourceAddContactRelationshipContact

Required when the new member of the community is not a registered contact so basic contact informaiton is required to be filled in. Applicable only for non-registered contacts.

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceAddContactRelationshipContact } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceAddContactRelationshipContact = {
  firstName: "Constantin",
  lastName: "Maggio",
  phone: {
    countryCode: "CYP",
    number: "744444121",
  },
};
```

## Fields

| Field                                                                                                                                                                                    | Type                                                                                                                                                                                     | Required                                                                                                                                                                                 | Description                                                                                                                                                                              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `firstName`                                                                                                                                                                              | *string*                                                                                                                                                                                 | :heavy_check_mark:                                                                                                                                                                       | The contact first name                                                                                                                                                                   |
| `lastName`                                                                                                                                                                               | *string*                                                                                                                                                                                 | :heavy_check_mark:                                                                                                                                                                       | The contact last name                                                                                                                                                                    |
| `emailAddress`                                                                                                                                                                           | *string*                                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                                       | The contact email address                                                                                                                                                                |
| `phone`                                                                                                                                                                                  | [operations.ComCrmContactSelfServiceResourceAddContactRelationshipContactPhone](../../models/operations/com-crm-contact-self-service-resource-add-contact-relationship-contact-phone.md) | :heavy_minus_sign:                                                                                                                                                                       | The contact phone                                                                                                                                                                        |