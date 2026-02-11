# ComCrmIndustrySelfServiceResourceListIndustriesRequest

## Example Usage

```typescript
import { ComCrmIndustrySelfServiceResourceListIndustriesRequest } from "crmcom/models/operations";

let value: ComCrmIndustrySelfServiceResourceListIndustriesRequest = {
  name: "Education",
  page: 20,
  size: 20,
};
```

## Fields

| Field                                                   | Type                                                    | Required                                                | Description                                             | Example                                                 |
| ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- |
| `name`                                                  | *string*                                                | :heavy_minus_sign:                                      | The name of the industry                                | Education                                               |
| `order`                                                 | *string*                                                | :heavy_minus_sign:                                      | Defines how the results will be ordered<br/>Default: DESC |                                                         |
| `page`                                                  | *number*                                                | :heavy_minus_sign:                                      | The page number that should be retrieved<br/>Default: 1 | 20                                                      |
| `size`                                                  | *number*                                                | :heavy_minus_sign:                                      | The size (total records) of each page<br/>Default: 10   | 20                                                      |
| `sort`                                                  | *string*                                                | :heavy_minus_sign:                                      | Defines on which attribute the results should be sorted |                                                         |