# GiftSender

Gift sender information

## Example Usage

```typescript
import { GiftSender } from "crmcom/models/operations";

let value: GiftSender = {
  name: "Kelly Smith",
  message: "Happy birthday John, have a great day. Hope to see you soon. Kelly",
};
```

## Fields

| Field                                                              | Type                                                               | Required                                                           | Description                                                        | Example                                                            |
| ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ |
| `name`                                                             | *string*                                                           | :heavy_check_mark:                                                 | Gift sender name                                                   | Kelly Smith                                                        |
| `message`                                                          | *string*                                                           | :heavy_minus_sign:                                                 | A short message from the gift sender to accompany the gift pass    | Happy birthday John, have a great day. Hope to see you soon. Kelly |