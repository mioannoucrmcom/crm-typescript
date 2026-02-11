# DemoContactContact

The contact that will be assigned as demo contact (required only if demo contact is enabled)

## Example Usage

```typescript
import { DemoContactContact } from "crmcom/models/operations";

let value: DemoContactContact = {
  id: "76ee374d-cd38-4cde-9fa3-4eaa26e67a06",
  name: "John Doe",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `id`                                 | *string*                             | :heavy_minus_sign:                   | The (demo) contact identifier        | 76ee374d-cd38-4cde-9fa3-4eaa26e67a06 |
| `name`                               | *string*                             | :heavy_minus_sign:                   | The (demo) contact full name         | John Doe                             |