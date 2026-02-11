# RegisteredContact

Details required if the pass is being created for a registered contact.

## Example Usage

```typescript
import { RegisteredContact } from "crmcom/models/operations";

let value: RegisteredContact = {
  contactId: "acaae121-b4af-4663-8646-47bb541c971d",
  walletId: "4613eb36-e5e8-46e8-9517-b1a31e86c89c",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `contactId`                          | *string*                             | :heavy_check_mark:                   | The existing contact's unique id     | acaae121-b4af-4663-8646-47bb541c971d |
| `walletId`                           | *string*                             | :heavy_check_mark:                   | Wallet id of the existing contact    | 4613eb36-e5e8-46e8-9517-b1a31e86c89c |