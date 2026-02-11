# ComCrmPaymentSelfServiceResourceCreatePaymentMethod

Payment method to be used to collect the money

## Example Usage

```typescript
import { ComCrmPaymentSelfServiceResourceCreatePaymentMethod } from "crm/models/operations";

let value: ComCrmPaymentSelfServiceResourceCreatePaymentMethod = {
  id: "CAD1E31269B76D7A65ACCE45B2E68DFD",
};
```

## Fields

| Field                                                                                                                                         | Type                                                                                                                                          | Required                                                                                                                                      | Description                                                                                                                                   | Example                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                          | *string*                                                                                                                                      | :heavy_minus_sign:                                                                                                                            | Contact payment method identifier. Applicable and requied when an online paymen tmethod tyoe is selected i.e. Card, Accoount Debit or Wallet. | CAD1E31269B76D7A65ACCE45B2E68DFD                                                                                                              |
| `type`                                                                                                                                        | [operations.ComCrmPaymentSelfServiceResourceCreateType](../../models/operations/com-crm-payment-self-service-resource-create-type.md)         | :heavy_minus_sign:                                                                                                                            | The payment method type                                                                                                                       |                                                                                                                                               |