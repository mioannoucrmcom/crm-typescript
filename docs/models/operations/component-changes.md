# ComponentChanges

## Example Usage

```typescript
import { ComponentChanges } from "crm/models/operations";

let value: ComponentChanges = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  toBeAdded: [
    {
      productId: "2dc0809f-ed91-4b68-b912-5bd6064d901e",
      priceTermsId: "32c0809f-ed91-4b68-b912-5bd6064d901e",
    },
  ],
  toBeRemoved: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    },
  ],
};
```

## Fields

| Field                                                                | Type                                                                 | Required                                                             | Description                                                          | Example                                                              |
| -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| `id`                                                                 | *string*                                                             | :heavy_minus_sign:                                                   | The entity identifier that will be created                           | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                 |
| `toBeAdded`                                                          | [operations.ToBeAdded](../../models/operations/to-be-added.md)[]     | :heavy_minus_sign:                                                   | N/A                                                                  |                                                                      |
| `toBeRemoved`                                                        | [operations.ToBeRemoved](../../models/operations/to-be-removed.md)[] | :heavy_minus_sign:                                                   | N/A                                                                  |                                                                      |