# ComCrmContactSelfServiceResourceGetPaymentMethodsContent

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetPaymentMethodsContent } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceGetPaymentMethodsContent = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  isPrimary: true,
  isRewards: true,
  paymentMethodType: "CARD",
  notes: "notes",
  name: "cash",
  card: {
    name: "Default Card",
    first6: "123456",
    last4: "4444",
    brand: "VISA",
    fundingType: "CREDIT",
    expirationMonth: 1,
    expirationYear: 2020,
    countryOfIssue: "CYP",
    cardHolderDetails: {
      cardHolderName: "John Doe",
      addressLine1: "Elia Papakyriakou",
      addressLine2: "7 Tower Star",
      addressCity: "Nicosia",
      addressZip: "2415",
      addressState: "Nicosia",
      addressCountry: "CYP",
      useBillingAddress: true,
    },
    gatewayToken: [
      {
        gateway: "JCC",
        token: "Xt5EWLLDS7FJjR1c",
        integration: {
          id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
          name: "Universal Name",
        },
      },
    ],
  },
  accountDebit: {
    accountName: "debit",
    accountNumber: "001002001",
    iban: "0143240434320434",
    sortCode: "20-02-53",
    routingNumber: "3425425253",
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
        gateway: "JCC",
        token: "Xt5EWLLDS7FJjR1c",
        integration: {
          id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
          name: "Universal Name",
        },
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
  wallet: {
    phone: null,
    email: "jsmith@email.com",
    gatewayToken: [
      {
        gateway: "JCC",
        token: "Xt5EWLLDS7FJjR1c",
        integration: {
          id: "34b059a3-2aa7-b2c2-4191-a966168e97d7",
          name: "Universal Name",
        },
      },
    ],
  },
  a2a: {
    schemeName: "BECSElectronicCredit",
    accountIdentification: "99-7354-1340583-01",
    currency: "NZD",
    accountName: "CurrentAccount",
    gatewayToken: [
      {
        gateway: "JCC",
        token: "Xt5EWLLDS7FJjR1c",
        integration: null,
      },
    ],
  },
};
```

## Fields

| Field                                                                                                                                                                                                  | Type                                                                                                                                                                                                   | Required                                                                                                                                                                                               | Description                                                                                                                                                                                            | Example                                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                                                                                                                   | *string*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | The entity identifier                                                                                                                                                                                  | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                   |
| `isPrimary`                                                                                                                                                                                            | *boolean*                                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                     | Indicates which payment mehod is the contact’s primary one                                                                                                                                             | true                                                                                                                                                                                                   |
| `isRewards`                                                                                                                                                                                            | *boolean*                                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                     | Defines whether the payment method is used only for identification purposes when a purchase is submitted (i.e. identify a contact with such card and not be able to be used on financial transactions) | true                                                                                                                                                                                                   |
| `paymentMethodId`                                                                                                                                                                                      | *string*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | The payment method’s identifier                                                                                                                                                                        |                                                                                                                                                                                                        |
| `paymentMethodType`                                                                                                                                                                                    | [operations.ComCrmContactSelfServiceResourceGetPaymentMethodsPaymentMethodType](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-payment-method-type.md)              | :heavy_minus_sign:                                                                                                                                                                                     | The type of the event                                                                                                                                                                                  | CARD                                                                                                                                                                                                   |
| `notes`                                                                                                                                                                                                | *string*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | The notes for payment methods                                                                                                                                                                          | notes                                                                                                                                                                                                  |
| `name`                                                                                                                                                                                                 | *string*                                                                                                                                                                                               | :heavy_minus_sign:                                                                                                                                                                                     | The name for payment methods                                                                                                                                                                           | cash                                                                                                                                                                                                   |
| `card`                                                                                                                                                                                                 | [operations.ComCrmContactSelfServiceResourceGetPaymentMethodsCard](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-card.md)                                          | :heavy_minus_sign:                                                                                                                                                                                     | The card’s main information. Required and applicable if the payment method type is CARD                                                                                                                |                                                                                                                                                                                                        |
| `accountDebit`                                                                                                                                                                                         | [operations.ComCrmContactSelfServiceResourceGetPaymentMethodsAccountDebit](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-account-debit.md)                         | :heavy_minus_sign:                                                                                                                                                                                     | The bank details.Required and applicable if the payment method is set to BANK                                                                                                                          |                                                                                                                                                                                                        |
| `wallet`                                                                                                                                                                                               | [operations.ComCrmContactSelfServiceResourceGetPaymentMethodsWallet](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-wallet.md)                                      | :heavy_minus_sign:                                                                                                                                                                                     | The wallet's main information. Required and applicable if the payment method type is WALLET                                                                                                            |                                                                                                                                                                                                        |
| `classification`                                                                                                                                                                                       | [operations.ComCrmContactSelfServiceResourceGetPaymentMethodsContentClassification](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-content-classification.md)       | :heavy_minus_sign:                                                                                                                                                                                     | Defines whether the payment method is related to a contact and/or wallet                                                                                                                               |                                                                                                                                                                                                        |
| `a2a`                                                                                                                                                                                                  | [operations.A2a](../../models/operations/a2a.md)                                                                                                                                                       | :heavy_minus_sign:                                                                                                                                                                                     | The account details.Required and applicable if the payment method is set to A2A                                                                                                                        |                                                                                                                                                                                                        |