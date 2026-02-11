# AddContactTokenSSPurchase

The purchase that will be approved (applicable if intent = APPROVE_PURCHASE)

## Example Usage

```typescript
import { AddContactTokenSSPurchase } from "crmcom/models/operations";

let value: AddContactTokenSSPurchase = {
  estimateId: "813cd698-e413-ce41-f543-0561144bbca9",
};
```

## Fields

| Field                                                    | Type                                                     | Required                                                 | Description                                              | Example                                                  |
| -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- |
| `estimateId`                                             | *string*                                                 | :heavy_check_mark:                                       | The purchase estimate (identifier) that will be approved | 813cd698-e413-ce41-f543-0561144bbca9                     |