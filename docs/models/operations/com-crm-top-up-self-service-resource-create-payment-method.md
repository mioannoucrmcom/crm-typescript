# ComCrmTopUpSelfServiceResourceCreatePaymentMethod

The top up’s payment method

## Example Usage

```typescript
import { ComCrmTopUpSelfServiceResourceCreatePaymentMethod } from "crmcom/models/operations";

let value: ComCrmTopUpSelfServiceResourceCreatePaymentMethod = {
  id: "e283a863-18e1-7cae-48c4-7433bf28cf97",
};
```

## Fields

| Field                                                                                                                              | Type                                                                                                                               | Required                                                                                                                           | Description                                                                                                                        | Example                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                               | *string*                                                                                                                           | :heavy_minus_sign:                                                                                                                 | The ID of the actual payment method, if any. Applicable only when the wallet is toped-up using a Card                              | e283a863-18e1-7cae-48c4-7433bf28cf97                                                                                               |
| `type`                                                                                                                             | [operations.ComCrmTopUpSelfServiceResourceCreateType](../../models/operations/com-crm-top-up-self-service-resource-create-type.md) | :heavy_minus_sign:                                                                                                                 | The payment method                                                                                                                 |                                                                                                                                    |