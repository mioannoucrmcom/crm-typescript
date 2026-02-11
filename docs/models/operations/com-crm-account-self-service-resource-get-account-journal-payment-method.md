# ComCrmAccountSelfServiceResourceGetAccountJournalPaymentMethod

Payment method details (e.g. for a refund)

## Example Usage

```typescript
import { ComCrmAccountSelfServiceResourceGetAccountJournalPaymentMethod } from "crmcom/models/operations";

let value: ComCrmAccountSelfServiceResourceGetAccountJournalPaymentMethod = {
  identity: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    identifier: "Visa *****1234 03/25",
  },
};
```

## Fields

| Field                                                                                                                                                                 | Type                                                                                                                                                                  | Required                                                                                                                                                              | Description                                                                                                                                                           | Example                                                                                                                                                               |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `type`                                                                                                                                                                | [operations.ComCrmAccountSelfServiceResourceGetAccountJournalType](../../models/operations/com-crm-account-self-service-resource-get-account-journal-type.md)         | :heavy_minus_sign:                                                                                                                                                    | type of payment method                                                                                                                                                |                                                                                                                                                                       |
| `identity`                                                                                                                                                            | [operations.ComCrmAccountSelfServiceResourceGetAccountJournalIdentity](../../models/operations/com-crm-account-self-service-resource-get-account-journal-identity.md) | :heavy_minus_sign:                                                                                                                                                    | An identifier that briefly describes the contact’s payment method (The last 4 digits for cards, the email for Paypal accounts or the wallet number                    | ****1234                                                                                                                                                              |