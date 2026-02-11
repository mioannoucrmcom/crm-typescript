# ComCrmApplicationSelfServiceResourceGetApplicationTransfer

Defines the supported transfer features

## Example Usage

```typescript
import { ComCrmApplicationSelfServiceResourceGetApplicationTransfer } from "crm/models/operations";

let value: ComCrmApplicationSelfServiceResourceGetApplicationTransfer = {
  commercePools: [
    {
      id: "dc01f65b-a482-48f1-9fda-c163df72f28f",
      name: "Redeem Anywhere",
      description: "Ability to redeem on any organisation/day/product",
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                             | Type                                                                                                                                                                              | Required                                                                                                                                                                          | Description                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `isSupported`                                                                                                                                                                     | *boolean*                                                                                                                                                                         | :heavy_minus_sign:                                                                                                                                                                | Defines whether transfer is supported or not                                                                                                                                      |
| `transferEntity`                                                                                                                                                                  | [operations.TransferEntity](../../models/operations/transfer-entity.md)[]                                                                                                         | :heavy_minus_sign:                                                                                                                                                                | Defines on which entity the transfer will be issued against (wallet and/or account)                                                                                               |
| `transferRestrictions`                                                                                                                                                            | [operations.TransferRestriction](../../models/operations/transfer-restriction.md)[]                                                                                               | :heavy_minus_sign:                                                                                                                                                                | Defines whether wallet transfers will be applied on open and/or commerce balances (applicable & required only when wallet transfers are enabled)                                  |
| `commercePools`                                                                                                                                                                   | [operations.ComCrmApplicationSelfServiceResourceGetApplicationCommercePool](../../models/operations/com-crm-application-self-service-resource-get-application-commerce-pool.md)[] | :heavy_minus_sign:                                                                                                                                                                | Defines which commerce pools will be allowed for wallet transfers (applicable & required only when wallet transfers against commerce balance are enabled)                         |