# B2bDetails

Details about commerce pool promote & join information

## Example Usage

```typescript
import { B2bDetails } from "crm/models/operations";

let value: B2bDetails = {
  isPublished: true,
  isPromoted: true,
  promotedOrganisation: {
    id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
    name: "Universal Name",
  },
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         | Example                                                                             |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `isPublished`                                                                       | *boolean*                                                                           | :heavy_minus_sign:                                                                  | Defines whether the commerce pool is published to other organisations or not        | true                                                                                |
| `isPromoted`                                                                        | *boolean*                                                                           | :heavy_minus_sign:                                                                  | Defines whether the commerce pool is promoted from other organisations or not       | true                                                                                |
| `promotedOrganisation`                                                              | [operations.PromotedOrganisation](../../models/operations/promoted-organisation.md) | :heavy_minus_sign:                                                                  | The organisation from which the commerce pool was published                         |                                                                                     |