# DemoContact

The contact assigned as demo contact (used for app store verification purposes)

## Example Usage

```typescript
import { DemoContact } from "crmcom/models/operations";

let value: DemoContact = {
  isSupported: true,
  contact: {
    id: "76ee374d-cd38-4cde-9fa3-4eaa26e67a06",
    name: "John Doe",
  },
  otp: "123456",
};
```

## Fields

| Field                                                                                                       | Type                                                                                                        | Required                                                                                                    | Description                                                                                                 | Example                                                                                                     |
| ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `isSupported`                                                                                               | *boolean*                                                                                                   | :heavy_minus_sign:                                                                                          | Defines whether demo contact is supported or not                                                            | true                                                                                                        |
| `contact`                                                                                                   | [operations.DemoContactContact](../../models/operations/demo-contact-contact.md)                            | :heavy_minus_sign:                                                                                          | The contact that will be assigned as demo contact (required only if demo contact is enabled)                |                                                                                                             |
| `otp`                                                                                                       | *string*                                                                                                    | :heavy_minus_sign:                                                                                          | The one-time password that will be accepted for sign-in purposes (required only if demo contact is enabled) | 123456                                                                                                      |