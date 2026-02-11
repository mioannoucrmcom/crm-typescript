# ComCrmContactSelfServiceResourceUpdatePaymentMethodRequestBody

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceUpdatePaymentMethodRequestBody } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceUpdatePaymentMethodRequestBody = {
  isPrimary: true,
  notes: "notes",
  accountDebit: {
    accountName: "test124221",
    accountNumber: "01010100101001",
    iban: "0143240434320434",
    sortCode: "20-02-53",
    routingNumber: "34234525234",
    bank: "Barclays",
    bankCode: "0032933-1123",
    branch: "Ascot",
    swift: "12345678",
    accountType: "SAVINGS",
    mandate: {
      signDate: 1654756878,
      terminationDate: 1654756878,
    },
    gatewayToken: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        gateway: "JCC",
        token: "Xt5EWLLDS7FJjR1c",
        alternativeToken: "Xt5EWLLDS7FJjR1c",
        integrationId: "bce504a4-f712-5262-183c-f58218a7a0ed",
      },
    ],
    accountHolderDetails: {
      accountHolderName: "John Peterson",
      addressLine1: "Elia Papakyriakou",
      addressLine2: "7 Tower Star",
      addressCity: "Nicosia",
      addressZip: "2415",
      addressState: "Nicosia",
      addressCountry: "CYP",
    },
    country: "CYP",
    currency: "EUR",
  },
  card: {
    expMonth: 2,
    expYear: 2022,
    alternativeToken: "Xt5EWLLDS7FJjR1c",
    integrationId: "bce504a4-f712-5262-183c-f58218a7a0ed",
  },
};
```

## Fields

| Field                                                                                                                                                                              | Type                                                                                                                                                                               | Required                                                                                                                                                                           | Description                                                                                                                                                                        | Example                                                                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `name`                                                                                                                                                                             | *string*                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                 | The name of payment method                                                                                                                                                         |                                                                                                                                                                                    |
| `isPrimary`                                                                                                                                                                        | *boolean*                                                                                                                                                                          | :heavy_minus_sign:                                                                                                                                                                 | Marks the payment method as the contact’s primary one                                                                                                                              | true                                                                                                                                                                               |
| `notes`                                                                                                                                                                            | *string*                                                                                                                                                                           | :heavy_minus_sign:                                                                                                                                                                 | Notes related to te payment method                                                                                                                                                 | notes                                                                                                                                                                              |
| `accountDebit`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceUpdatePaymentMethodAccountDebit](../../models/operations/com-crm-contact-self-service-resource-update-payment-method-account-debit.md) | :heavy_minus_sign:                                                                                                                                                                 | The bank details. Required and applicable if the payment method is set to BANK                                                                                                     |                                                                                                                                                                                    |
| `card`                                                                                                                                                                             | [operations.ComCrmContactSelfServiceResourceUpdatePaymentMethodCard](../../models/operations/com-crm-contact-self-service-resource-update-payment-method-card.md)                  | :heavy_minus_sign:                                                                                                                                                                 | Applicable only when updating a payment method of type Card                                                                                                                        |                                                                                                                                                                                    |