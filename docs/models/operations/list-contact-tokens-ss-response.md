# ListContactTokensSSResponse

OK

## Example Usage

```typescript
import { ListContactTokensSSResponse } from "crm/models/operations";

let value: ListContactTokensSSResponse = {
  content: [
    {
      id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      value: "123456",
      alternativeToken: "8329123456789012",
      expiration: 1596714307,
      spendAmount: 14.52,
    },
  ],
};
```

## Fields

| Field                                                                                                | Type                                                                                                 | Required                                                                                             | Description                                                                                          |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `content`                                                                                            | [operations.ListContactTokensSSContent](../../models/operations/list-contact-tokens-ss-content.md)[] | :heavy_minus_sign:                                                                                   | N/A                                                                                                  |