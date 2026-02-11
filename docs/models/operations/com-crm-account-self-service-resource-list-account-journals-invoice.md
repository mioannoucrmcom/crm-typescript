# ComCrmAccountSelfServiceResourceListAccountJournalsInvoice

Invoice related details, applicable for invoice only

## Example Usage

```typescript
import { ComCrmAccountSelfServiceResourceListAccountJournalsInvoice } from "crm/models/operations";

let value: ComCrmAccountSelfServiceResourceListAccountJournalsInvoice = {
  dueDate: 1232412,
  overdueAmount: 15,
  unpaidAmount: 15,
};
```

## Fields

| Field                                                        | Type                                                         | Required                                                     | Description                                                  | Example                                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `dueDate`                                                    | *number*                                                     | :heavy_minus_sign:                                           | Invoice due date                                             | 1232412                                                      |
| `overdueAmount`                                              | *number*                                                     | :heavy_minus_sign:                                           | Invoice overdue amount                                       | 15                                                           |
| `unpaidAmount`                                               | *number*                                                     | :heavy_minus_sign:                                           | Invoice unpaid amount, i.e. invoice due date not yet reached | 15                                                           |