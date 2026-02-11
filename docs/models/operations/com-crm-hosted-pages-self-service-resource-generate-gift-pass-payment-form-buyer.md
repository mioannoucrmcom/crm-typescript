# ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormBuyer

Details about the buyer

## Example Usage

```typescript
import { ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormBuyer } from "crm/models/operations";

let value:
  ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormBuyer = {
    name: "<value>",
    phone: {
      countryCode: "CYP",
      number: "22265566",
    },
  };
```

## Fields

| Field                                                                                                                                                                                              | Type                                                                                                                                                                                               | Required                                                                                                                                                                                           | Description                                                                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `name`                                                                                                                                                                                             | *string*                                                                                                                                                                                           | :heavy_check_mark:                                                                                                                                                                                 | The buyer's name                                                                                                                                                                                   |
| `email`                                                                                                                                                                                            | *string*                                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                                 | The buyer's email address                                                                                                                                                                          |
| `phone`                                                                                                                                                                                            | [operations.ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormPhone](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-gift-pass-payment-form-phone.md)     | :heavy_minus_sign:                                                                                                                                                                                 | The buyer's phone                                                                                                                                                                                  |
| `address`                                                                                                                                                                                          | [operations.ComCrmHostedPagesSelfServiceResourceGenerateGiftPassPaymentFormAddress](../../models/operations/com-crm-hosted-pages-self-service-resource-generate-gift-pass-payment-form-address.md) | :heavy_minus_sign:                                                                                                                                                                                 | The billing address                                                                                                                                                                                |