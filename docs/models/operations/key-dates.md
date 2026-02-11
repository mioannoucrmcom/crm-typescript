# KeyDates

## Example Usage

```typescript
import { KeyDates } from "crm/models/operations";

let value: KeyDates = {
  submittedOn: 1592809457,
  completedOn: 1592809457,
  cancelledOn: 1592809457,
  requestedDate: 1649337036,
  startedOn: 1649337036,
  estimatedFulfillment: {
    date: 1592809457,
    duration: 30,
    uot: "MINUTE",
  },
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         | Example                                                                             |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `submittedOn`                                                                       | *number*                                                                            | :heavy_minus_sign:                                                                  | Submitted date                                                                      | 1592809457                                                                          |
| `completedOn`                                                                       | *number*                                                                            | :heavy_minus_sign:                                                                  | Completion date                                                                     | 1592809457                                                                          |
| `cancelledOn`                                                                       | *number*                                                                            | :heavy_minus_sign:                                                                  | Cancellation date                                                                   | 1592809457                                                                          |
| `requestedDate`                                                                     | *number*                                                                            | :heavy_minus_sign:                                                                  | Date on which the cotact requested for the order to be actually delivered           | 1649337036                                                                          |
| `startedOn`                                                                         | *number*                                                                            | :heavy_minus_sign:                                                                  | Date when the Order's processing started                                            | 1649337036                                                                          |
| `estimatedFulfillment`                                                              | [operations.EstimatedFulfillment](../../models/operations/estimated-fulfillment.md) | :heavy_minus_sign:                                                                  | When the order is estimated to be fulfilled                                         |                                                                                     |