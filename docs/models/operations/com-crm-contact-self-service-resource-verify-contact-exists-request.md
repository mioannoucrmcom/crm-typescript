# ComCrmContactSelfServiceResourceVerifyContactExistsRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceVerifyContactExistsRequest } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceVerifyContactExistsRequest = {
  emailAddress: "john@gmail.com",
  phone: "99123456",
};
```

## Fields

| Field                                                                                              | Type                                                                                               | Required                                                                                           | Description                                                                                        | Example                                                                                            |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `emailAddress`                                                                                     | *string*                                                                                           | :heavy_minus_sign:                                                                                 | The email address used by the contact to register. Either email_address or phone must be provided. | john@gmail.com                                                                                     |
| `phone`                                                                                            | *string*                                                                                           | :heavy_minus_sign:                                                                                 | The phone used by the contact to register. Either email_address or phone must be provided          | 99123456                                                                                           |