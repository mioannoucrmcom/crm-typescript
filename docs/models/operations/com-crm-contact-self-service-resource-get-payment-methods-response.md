# ComCrmContactSelfServiceResourceGetPaymentMethodsResponse

OK

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetPaymentMethodsResponse } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceGetPaymentMethodsResponse = {
  paging: {
    page: 2,
    size: 20,
    total: 5124,
    hasMore: true,
  },
  content: [
    {
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
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                 | Type                                                                                                                                                                  | Required                                                                                                                                                              | Description                                                                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `paging`                                                                                                                                                              | [operations.ComCrmContactSelfServiceResourceGetPaymentMethodsPaging](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-paging.md)     | :heavy_minus_sign:                                                                                                                                                    | N/A                                                                                                                                                                   |
| `content`                                                                                                                                                             | [operations.ComCrmContactSelfServiceResourceGetPaymentMethodsContent](../../models/operations/com-crm-contact-self-service-resource-get-payment-methods-content.md)[] | :heavy_minus_sign:                                                                                                                                                    | N/A                                                                                                                                                                   |