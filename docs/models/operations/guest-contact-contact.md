# GuestContactContact

The contact that will be assigned as guest contact (required only if guest contact is enabled)

## Example Usage

```typescript
import { GuestContactContact } from "crmcom/models/operations";

let value: GuestContactContact = {
  id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
  name: "John Doe",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `id`                                 | *string*                             | :heavy_minus_sign:                   | The (guest) contact identifier       | 34b059a3-2aa7-b2c2-4191-a966168e97d7 |
| `name`                               | *string*                             | :heavy_minus_sign:                   | The (guest) contact full name        | John Doe                             |