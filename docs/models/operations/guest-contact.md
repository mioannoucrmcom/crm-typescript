# GuestContact

The contact assigned as guest contact (used for continuing as guest in app)

## Example Usage

```typescript
import { GuestContact } from "crm/models/operations";

let value: GuestContact = {
  isSupported: true,
  contact: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "John Doe",
  },
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    | Example                                                                                        |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `isSupported`                                                                                  | *boolean*                                                                                      | :heavy_minus_sign:                                                                             | Defines whether guest contact is supported or not                                              | true                                                                                           |
| `contact`                                                                                      | [operations.GuestContactContact](../../models/operations/guest-contact-contact.md)             | :heavy_minus_sign:                                                                             | The contact that will be assigned as guest contact (required only if guest contact is enabled) |                                                                                                |