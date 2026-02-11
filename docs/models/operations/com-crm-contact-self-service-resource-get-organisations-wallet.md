# ComCrmContactSelfServiceResourceGetOrganisationsWallet

Contact wallet information for the organisation

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetOrganisationsWallet } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceGetOrganisationsWallet = {
  walletId: "038af54e-282c-40ad-ae5d-cc74f2c80f40",
  balance: 9.99,
  currencyCode: "EUR",
};
```

## Fields

| Field                                                      | Type                                                       | Required                                                   | Description                                                | Example                                                    |
| ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- |
| `walletId`                                                 | *string*                                                   | :heavy_minus_sign:                                         | Wallet id                                                  | 038af54e-282c-40ad-ae5d-cc74f2c80f40                       |
| `balance`                                                  | *number*                                                   | :heavy_minus_sign:                                         | Total of the open balance + commerce balance of the wallet | 9.99                                                       |
| `currencyCode`                                             | *string*                                                   | :heavy_minus_sign:                                         | The currency code                                          | EUR                                                        |