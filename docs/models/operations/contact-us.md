# ContactUs

The application "contact us" details

## Example Usage

```typescript
import { ContactUs } from "crm/models/operations";

let value: ContactUs = {
  emailAddress: "info@crm.com",
  phone: {
    countryCode: "CYP",
    number: "22265566",
  },
  website: "https?/crm.com",
};
```

## Fields

| Field                                                                                                                                                            | Type                                                                                                                                                             | Required                                                                                                                                                         | Description                                                                                                                                                      | Example                                                                                                                                                          |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `emailAddress`                                                                                                                                                   | *string*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | The contact us email address                                                                                                                                     | info@crm.com                                                                                                                                                     |
| `phone`                                                                                                                                                          | [operations.ComCrmApplicationSelfServiceResourceGetApplicationPhone](../../models/operations/com-crm-application-self-service-resource-get-application-phone.md) | :heavy_minus_sign:                                                                                                                                               | The contact us phone                                                                                                                                             |                                                                                                                                                                  |
| `website`                                                                                                                                                        | *string*                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                               | The contact us website                                                                                                                                           | https?/crm.com                                                                                                                                                   |