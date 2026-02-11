# Components

Applicable when amending a service bundle. At least one components to be added or to be removed must be specified

## Example Usage

```typescript
import { Components } from "crmcom/models/operations";

let value: Components = {
  added: [
    {
      productId: "2dc0809f-ed91-4b68-b912-5bd6064d901e",
      priceTermsId: "32c0809f-ed91-4b68-b912-5bd6064d901e",
    },
  ],
  removed: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    },
  ],
};
```

## Fields

| Field                                                      | Type                                                       | Required                                                   | Description                                                |
| ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- |
| `added`                                                    | [operations.Added](../../models/operations/added.md)[]     | :heavy_minus_sign:                                         | Component services to be added                             |
| `removed`                                                  | [operations.Removed](../../models/operations/removed.md)[] | :heavy_minus_sign:                                         | Component services to be removed                           |