# ComCrmContactSelfServiceResourceAddPaymentMethodRequestBody

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceAddPaymentMethodRequestBody } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceAddPaymentMethodRequestBody = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "PayPal",
  isPrimary: true,
  paymentMethodType: "CASH",
  notes: "Lorem Ipsum",
  card: null,
  wallet: {
    phoneDetails: null,
    email: "jsmith@email.com",
    name: "John Smith",
    gatewayToken: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
        gateway: "JCC",
        token: "Xt5EWLLDS7FJjR1c",
        alternativeToken: "Xt5EWLLDS7FJjR1c",
        integrationId: "bce504a4-f712-5262-183c-f58218a7a0ed",
      },
    ],
  },
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
};
```

## Fields

| Field                                                                                                                                                                                   | Type                                                                                                                                                                                    | Required                                                                                                                                                                                | Description                                                                                                                                                                             | Example                                                                                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                    | *string*                                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                      | The entity identifier that will be created                                                                                                                                              | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                    |
| `name`                                                                                                                                                                                  | *string*                                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                      | A name that provides a small description for the payment method. In case of Wallet payment method types, use the Payment Gateway’s name                                                 | PayPal                                                                                                                                                                                  |
| `contactId`                                                                                                                                                                             | *string*                                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                      | the contact for the payment method                                                                                                                                                      |                                                                                                                                                                                         |
| `isPrimary`                                                                                                                                                                             | *boolean*                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                      | Marks the payment method as the contact’s primary one                                                                                                                                   | true                                                                                                                                                                                    |
| `paymentMethodType`                                                                                                                                                                     | [operations.ComCrmContactSelfServiceResourceAddPaymentMethodPaymentMethodType](../../models/operations/com-crm-contact-self-service-resource-add-payment-method-payment-method-type.md) | :heavy_minus_sign:                                                                                                                                                                      | The payment method that will be related with the account                                                                                                                                | CASH                                                                                                                                                                                    |
| `notes`                                                                                                                                                                                 | *string*                                                                                                                                                                                | :heavy_minus_sign:                                                                                                                                                                      | Notes related to te payment method                                                                                                                                                      | Lorem Ipsum                                                                                                                                                                             |
| `card`                                                                                                                                                                                  | [operations.ComCrmContactSelfServiceResourceAddPaymentMethodCard](../../models/operations/com-crm-contact-self-service-resource-add-payment-method-card.md)                             | :heavy_check_mark:                                                                                                                                                                      | The card details (required and applicable if the payment method is set to CARD)                                                                                                         |                                                                                                                                                                                         |
| `wallet`                                                                                                                                                                                | [operations.ComCrmContactSelfServiceResourceAddPaymentMethodWallet](../../models/operations/com-crm-contact-self-service-resource-add-payment-method-wallet.md)                         | :heavy_check_mark:                                                                                                                                                                      | The phone details (required and applicable if the payment method is set to PHONE)                                                                                                       |                                                                                                                                                                                         |
| `accountDebit`                                                                                                                                                                          | [operations.ComCrmContactSelfServiceResourceAddPaymentMethodAccountDebit](../../models/operations/com-crm-contact-self-service-resource-add-payment-method-account-debit.md)            | :heavy_check_mark:                                                                                                                                                                      | The bank details (required and applicable if the payment method is set to BANK)                                                                                                         |                                                                                                                                                                                         |