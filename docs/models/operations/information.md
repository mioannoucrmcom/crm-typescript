# Information

Defines the app details (about, terms and conditions, privacy policy)

## Example Usage

```typescript
import { Information } from "crmcom/models/operations";

let value: Information = {
  content: [
    {
      url: "https?/crm.com",
      richContent: "Terms & Conditions",
    },
  ],
  contactUs: {
    emailAddress: "info@crm.com",
    phone: {
      countryCode: "CYP",
      number: "22265566",
    },
    website: "https?/crm.com",
  },
};
```

## Fields

| Field                                                                                                                                                                  | Type                                                                                                                                                                   | Required                                                                                                                                                               | Description                                                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `content`                                                                                                                                                              | [operations.ComCrmApplicationSelfServiceResourceGetApplicationContent](../../models/operations/com-crm-application-self-service-resource-get-application-content.md)[] | :heavy_minus_sign:                                                                                                                                                     | The application content information                                                                                                                                    |
| `contactUs`                                                                                                                                                            | [operations.ContactUs](../../models/operations/contact-us.md)                                                                                                          | :heavy_minus_sign:                                                                                                                                                     | The application "contact us" details                                                                                                                                   |