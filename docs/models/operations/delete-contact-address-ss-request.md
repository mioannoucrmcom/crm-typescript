# DeleteContactAddressSSRequest

## Example Usage

```typescript
import { DeleteContactAddressSSRequest } from "crm/models/operations";

let value: DeleteContactAddressSSRequest = {
  addressId: "cadbf723-fdc6-4598-8156-f6288e61f356",
  id: "1a6a85ac-aacf-4175-8de2-a7d701186d96",
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         | Example                                             |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `addressId`                                         | *string*                                            | :heavy_check_mark:                                  | The id of the address to be deleted                 | cadbf723-fdc6-4598-8156-f6288e61f356                |
| `id`                                                | *string*                                            | :heavy_check_mark:                                  | The contact id for which an address will be deleted | 1a6a85ac-aacf-4175-8de2-a7d701186d96                |