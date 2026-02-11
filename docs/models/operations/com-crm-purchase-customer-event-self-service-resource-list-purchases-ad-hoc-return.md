# ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesAdHocReturn

Details about the ad hoc return of goods that is associated with the purchase

## Example Usage

```typescript
import { ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesAdHocReturn } from "crm/models/operations";

let value:
  ComCrmPurchaseCustomerEventSelfServiceResourceListPurchasesAdHocReturn = {
    amount: 12.34,
    date: 1589987160,
    referenceNumber: "AHR001",
    returnAmount: 200.99,
    returnSpentAmount: 200.99,
  };
```

## Fields

| Field                                                                                                   | Type                                                                                                    | Required                                                                                                | Description                                                                                             | Example                                                                                                 |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| `amount`                                                                                                | *number*                                                                                                | :heavy_minus_sign:                                                                                      | The amount that the contact was debited due to ad hoc return of goods                                   | 12.34                                                                                                   |
| `date`                                                                                                  | *number*                                                                                                | :heavy_minus_sign:                                                                                      | The date that ad hoc retun of goods was applied                                                         | 1589987160                                                                                              |
| `referenceNumber`                                                                                       | *string*                                                                                                | :heavy_minus_sign:                                                                                      | The ad hoc return reference number (usually a human-readable code issued by the POS & eCommerce system) | AHR001                                                                                                  |
| `returnAmount`                                                                                          | *number*                                                                                                | :heavy_minus_sign:                                                                                      | The amount that was returned                                                                            | 200.99                                                                                                  |
| `returnSpentAmount`                                                                                     | *number*                                                                                                | :heavy_minus_sign:                                                                                      | The spent amount that was returned                                                                      | 200.99                                                                                                  |