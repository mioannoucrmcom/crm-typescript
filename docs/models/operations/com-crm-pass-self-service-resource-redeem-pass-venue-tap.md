# ComCrmPassSelfServiceResourceRedeemPassVenueTap

The transaction acquiring point that the event was submitted from (id or code must be specified), usualy a unique number-based code

## Example Usage

```typescript
import { ComCrmPassSelfServiceResourceRedeemPassVenueTap } from "crm/models/operations";

let value: ComCrmPassSelfServiceResourceRedeemPassVenueTap = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  code: "2131424123",
};
```

## Fields

| Field                                | Type                                 | Required                             | Description                          | Example                              |
| ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ | ------------------------------------ |
| `id`                                 | *string*                             | :heavy_minus_sign:                   | The entity identifier                | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0 |
| `code`                               | *string*                             | :heavy_minus_sign:                   | The entity code                      | 2131424123                           |