# ComCrmPaymentFormSelfServiceResourceGeneratePassPaymentFormBuyer

Details about the buyer

## Example Usage

```typescript
import { ComCrmPaymentFormSelfServiceResourceGeneratePassPaymentFormBuyer } from "crmcom/models/operations";

let value: ComCrmPaymentFormSelfServiceResourceGeneratePassPaymentFormBuyer = {
  name: "<value>",
  phone: {
    countryCode: "CYP",
    number: "22265566",
  },
};
```

## Fields

| Field                                                                                                                                                                                     | Type                                                                                                                                                                                      | Required                                                                                                                                                                                  | Description                                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `name`                                                                                                                                                                                    | *string*                                                                                                                                                                                  | :heavy_check_mark:                                                                                                                                                                        | The buyer's name                                                                                                                                                                          |
| `email`                                                                                                                                                                                   | *string*                                                                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                                        | The buyer's email address                                                                                                                                                                 |
| `phone`                                                                                                                                                                                   | [operations.ComCrmPaymentFormSelfServiceResourceGeneratePassPaymentFormPhone](../../models/operations/com-crm-payment-form-self-service-resource-generate-pass-payment-form-phone.md)     | :heavy_minus_sign:                                                                                                                                                                        | The buyer's phone                                                                                                                                                                         |
| `address`                                                                                                                                                                                 | [operations.ComCrmPaymentFormSelfServiceResourceGeneratePassPaymentFormAddress](../../models/operations/com-crm-payment-form-self-service-resource-generate-pass-payment-form-address.md) | :heavy_minus_sign:                                                                                                                                                                        | The billing address                                                                                                                                                                       |