# UpdateContactAddressSSRequest

## Example Usage

```typescript
import { UpdateContactAddressSSRequest } from "crmcom/models/operations";

let value: UpdateContactAddressSSRequest = {
  addressId: "cadbf723-fdc6-4598-8156-f6288e61f356",
  id: "1a6a85ac-aacf-4175-8de2-a7d701186d96",
};
```

## Fields

| Field                                                                                                             | Type                                                                                                              | Required                                                                                                          | Description                                                                                                       | Example                                                                                                           |
| ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `addressId`                                                                                                       | *string*                                                                                                          | :heavy_check_mark:                                                                                                | The address identifier that will be updated                                                                       | cadbf723-fdc6-4598-8156-f6288e61f356                                                                              |
| `id`                                                                                                              | *string*                                                                                                          | :heavy_check_mark:                                                                                                | The contact identifier for which an address will be updated                                                       | 1a6a85ac-aacf-4175-8de2-a7d701186d96                                                                              |
| `body`                                                                                                            | [operations.UpdateContactAddressSSRequestBody](../../models/operations/update-contact-address-ss-request-body.md) | :heavy_minus_sign:                                                                                                | N/A                                                                                                               |                                                                                                                   |