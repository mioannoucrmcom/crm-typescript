# CreatedBy

Details of the user who created the note

## Example Usage

```typescript
import { CreatedBy } from "crmcom/models/operations";

let value: CreatedBy = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  username: "Sam Jackson",
  name: "S_Jackson",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `id`                                 | *string*                             | :heavy_minus_sign:                   | The entity identifier                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0 |
| `username`                           | *string*                             | :heavy_minus_sign:                   | The user's credential username       | Sam Jackson                          |
| `name`                               | *string*                             | :heavy_minus_sign:                   | The user's full name                 | S_Jackson                            |