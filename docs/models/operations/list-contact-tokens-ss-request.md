# ListContactTokensSSRequest

## Example Usage

```typescript
import { ListContactTokensSSRequest } from "crm/models/operations";

let value: ListContactTokensSSRequest = {
  id: "33749faa-4ef0-426d-f9f0-83b91bf5ab3f",
  communityId: "c1d2e3f4-5678-90ab-cdef-1234567890ab",
  intent: "SPEND",
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        | Example                                                                            |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `id`                                                                               | *string*                                                                           | :heavy_check_mark:                                                                 | The id of the contact whose tokens will be retrieved                               | 33749faa-4ef0-426d-f9f0-83b91bf5ab3f                                               |
| `communityId`                                                                      | *string*                                                                           | :heavy_minus_sign:                                                                 | The id of the community to which the contact which the contact wants to spend from | c1d2e3f4-5678-90ab-cdef-1234567890ab                                               |
| `intent`                                                                           | [operations.QueryParamIntent](../../models/operations/query-param-intent.md)       | :heavy_minus_sign:                                                                 | Filter based on the intent that tokens were requested                              | SPEND                                                                              |