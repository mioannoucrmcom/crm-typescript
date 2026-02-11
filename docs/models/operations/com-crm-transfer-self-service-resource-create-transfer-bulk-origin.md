# ComCrmTransferSelfServiceResourceCreateTransferBulkOrigin

The origin of the transfer. Can be either an account or a wallet

## Example Usage

```typescript
import { ComCrmTransferSelfServiceResourceCreateTransferBulkOrigin } from "crmcom/models/operations";

let value: ComCrmTransferSelfServiceResourceCreateTransferBulkOrigin = {
  accountId: "CAD1E31269B76D7A65ACCE45B2E68DFD",
  walletId: "A65ACCE45B2E68DFDCAD1E31269B76D7",
};
```

## Fields

| Field                            | Type                             | Required                         | Description                      | Example                          |
| -------------------------------- | -------------------------------- | -------------------------------- | -------------------------------- | -------------------------------- |
| `accountId`                      | *string*                         | :heavy_minus_sign:               | Account unique id                | CAD1E31269B76D7A65ACCE45B2E68DFD |
| `walletId`                       | *string*                         | :heavy_minus_sign:               | Wallet unique id                 | A65ACCE45B2E68DFDCAD1E31269B76D7 |