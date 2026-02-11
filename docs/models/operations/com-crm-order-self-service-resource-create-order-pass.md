# ComCrmOrderSelfServiceResourceCreateOrderPass

The details of the e-gift pass to be created.

## Example Usage

```typescript
import { ComCrmOrderSelfServiceResourceCreateOrderPass } from "crmcom/models/operations";

let value: ComCrmOrderSelfServiceResourceCreateOrderPass = {
  recipient: {
    name: "John Smith",
    mediumType: "EMAIL",
    mediumValue: "j.smith@crm.com",
    countryCode: "LBR",
    language: "EN",
    registeredContact: {
      contactId: "acaae121-b4af-4663-8646-47bb541c971d",
      walletId: "4613eb36-e5e8-46e8-9517-b1a31e86c89c",
    },
  },
  giftSender: {
    name: "Kelly Smith",
    message:
      "Happy birthday John, have a great day. Hope to see you soon. Kelly",
  },
};
```

## Fields

| Field                                                                                                  | Type                                                                                                   | Required                                                                                               | Description                                                                                            |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| `recipient`                                                                                            | [operations.Recipient](../../models/operations/recipient.md)                                           | :heavy_minus_sign:                                                                                     | The recipient information.This is the registered/unregistered contact who will be redeeming the pass.  |
| `giftSender`                                                                                           | [operations.GiftSender](../../models/operations/gift-sender.md)                                        | :heavy_minus_sign:                                                                                     | Gift sender information                                                                                |