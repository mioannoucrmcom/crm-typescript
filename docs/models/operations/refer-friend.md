# ReferFriend

Defines the supported refer a friend features

## Example Usage

```typescript
import { ReferFriend } from "crm/models/operations";

let value: ReferFriend = {
  isSupported: true,
};
```

## Fields

| Field                                                                   | Type                                                                    | Required                                                                | Description                                                             | Example                                                                 |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `isSupported`                                                           | *boolean*                                                               | :heavy_minus_sign:                                                      | Defines whether refer a friend will be supported                        | true                                                                    |
| `referMethods`                                                          | [operations.ReferMethod](../../models/operations/refer-method.md)[]     | :heavy_minus_sign:                                                      | Defines the communication method that should be used for refer a friend |                                                                         |