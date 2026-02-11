# SettlementEvent

Details about the event that initiated such settlement request

## Example Usage

```typescript
import { SettlementEvent } from "crm/models/operations";

let value: SettlementEvent = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  type: "PURCHASE",
  referenceNumber: "2833205645375343",
  amount: 102.79,
  postedDate: 1635170879,
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 | Example                                                                     |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `id`                                                                        | *string*                                                                    | :heavy_minus_sign:                                                          | The entity identifier                                                       | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                        |
| `type`                                                                      | [operations.TypePurchase](../../models/operations/type-purchase.md)         | :heavy_minus_sign:                                                          | Defines the type of the event that is related to the settlement transaction | PURCHASE                                                                    |
| `referenceNumber`                                                           | *string*                                                                    | :heavy_minus_sign:                                                          | The event reference number/code (if applicable)                             | 2833205645375343                                                            |
| `amount`                                                                    | *number*                                                                    | :heavy_minus_sign:                                                          | The event amount                                                            | 102.79                                                                      |
| `postedDate`                                                                | *number*                                                                    | :heavy_minus_sign:                                                          | The date on which the event was posted                                      | 1635170879                                                                  |
| `locationName`                                                              | *string*                                                                    | :heavy_minus_sign:                                                          | N/A                                                                         |                                                                             |