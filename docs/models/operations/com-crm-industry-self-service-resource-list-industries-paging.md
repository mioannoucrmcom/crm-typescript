# ComCrmIndustrySelfServiceResourceListIndustriesPaging

## Example Usage

```typescript
import { ComCrmIndustrySelfServiceResourceListIndustriesPaging } from "crmcom/models/operations";

let value: ComCrmIndustrySelfServiceResourceListIndustriesPaging = {
  page: 2,
  size: 20,
  total: 5124,
};
```

## Fields

| Field                                                     | Type                                                      | Required                                                  | Description                                               | Example                                                   |
| --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| `page`                                                    | *number*                                                  | :heavy_minus_sign:                                        | The page number                                           | 2                                                         |
| `size`                                                    | *number*                                                  | :heavy_minus_sign:                                        | The number of records per page                            | 20                                                        |
| `total`                                                   | *number*                                                  | :heavy_minus_sign:                                        | The overall number of records, only accurate up to 10,000 | 5124                                                      |