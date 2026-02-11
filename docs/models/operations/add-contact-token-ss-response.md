# AddContactTokenSSResponse

OK

## Example Usage

```typescript
import { AddContactTokenSSResponse } from "crmcom/models/operations";

let value: AddContactTokenSSResponse = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  value: "123456",
  alternativeToken: "8329123456789012",
  expiration: 1596714307,
  spendAmount: 14.52,
};
```

## Fields

| Field                                                               | Type                                                                | Required                                                            | Description                                                         | Example                                                             |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `id`                                                                | *string*                                                            | :heavy_minus_sign:                                                  | The entity identifier                                               | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                |
| `value`                                                             | *string*                                                            | :heavy_minus_sign:                                                  | The requested token                                                 | 123456                                                              |
| `alternativeToken`                                                  | *string*                                                            | :heavy_minus_sign:                                                  | A 16-digit numeric code that can be used instead of the token value | 8329123456789012                                                    |
| `expiration`                                                        | *number*                                                            | :heavy_minus_sign:                                                  | The token expiration date                                           | 1596714307                                                          |
| `spendAmount`                                                       | *number*                                                            | :heavy_minus_sign:                                                  | The amount requested to be spent                                    | 14.52                                                               |