# ComCrmContactSelfServiceResourceOptOutDonationsRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceOptOutDonationsRequest } from "crmcom/models/operations";

let value: ComCrmContactSelfServiceResourceOptOutDonationsRequest = {
  donationId: "ccc945d8-1bda-a11c-d378-23c29947c2a3",
  id: "5096c4d4-c387-9888-d631-80e74546e2db",
};
```

## Fields

| Field                                                              | Type                                                               | Required                                                           | Description                                                        | Example                                                            |
| ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------------------------ |
| `donationId`                                                       | *string*                                                           | :heavy_check_mark:                                                 | The donation offer (identifier) that the contact will opt out from | ccc945d8-1bda-a11c-d378-23c29947c2a3                               |
| `id`                                                               | *string*                                                           | :heavy_check_mark:                                                 | The contact (identifier) that will opt out from the donation offer | 5096c4d4-c387-9888-d631-80e74546e2db                               |