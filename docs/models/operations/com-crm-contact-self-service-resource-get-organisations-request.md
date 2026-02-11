# ComCrmContactSelfServiceResourceGetOrganisationsRequest

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceGetOrganisationsRequest } from "crm/models/operations";

let value: ComCrmContactSelfServiceResourceGetOrganisationsRequest = {
  id: "<id>",
  size: 100,
};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      | Example                                                                          |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `id`                                                                             | *string*                                                                         | :heavy_check_mark:                                                               | The contact (registry) (identifier) whose joined organisations will be retrieved |                                                                                  |
| `includeWallet`                                                                  | *boolean*                                                                        | :heavy_minus_sign:                                                               | Whether to include the wallet information of the contact for each organisation   |                                                                                  |
| `name`                                                                           | *string*                                                                         | :heavy_minus_sign:                                                               | The organisation name (should behave as like)                                    |                                                                                  |
| `page`                                                                           | *number*                                                                         | :heavy_minus_sign:                                                               | The page number that should be retrieved                                         | 1                                                                                |
| `size`                                                                           | *number*                                                                         | :heavy_minus_sign:                                                               | The size (total records) of each page                                            | 100                                                                              |