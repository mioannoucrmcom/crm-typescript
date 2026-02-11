# ComCrmServiceRequestSelfServiceResourceGetNotesContent

## Example Usage

```typescript
import { ComCrmServiceRequestSelfServiceResourceGetNotesContent } from "crm/models/operations";

let value: ComCrmServiceRequestSelfServiceResourceGetNotesContent = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  createdOn: 98765775,
  updatedOn: 98765775,
  createdBy: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    username: "Sam Jackson",
    name: "S_Jackson",
  },
  pinned: true,
  note:
    "After my telephone conversation with Zack this morning, it was decided that....",
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     | Example                                                                         |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `id`                                                                            | *string*                                                                        | :heavy_minus_sign:                                                              | The entity identifier                                                           | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                            |
| `createdOn`                                                                     | *number*                                                                        | :heavy_minus_sign:                                                              | Date and time the note was created                                              | 98765775                                                                        |
| `updatedOn`                                                                     | *number*                                                                        | :heavy_minus_sign:                                                              | Date and time the note was updated                                              | 98765775                                                                        |
| `createdBy`                                                                     | [operations.CreatedBy](../../models/operations/created-by.md)                   | :heavy_minus_sign:                                                              | Details of the user who created the note                                        |                                                                                 |
| `pinned`                                                                        | *boolean*                                                                       | :heavy_minus_sign:                                                              | Is note pinned so that it appears at the top of the notes list?                 | true                                                                            |
| `note`                                                                          | *string*                                                                        | :heavy_minus_sign:                                                              | The note contents                                                               | After my telephone conversation with Zack this morning, it was decided that.... |