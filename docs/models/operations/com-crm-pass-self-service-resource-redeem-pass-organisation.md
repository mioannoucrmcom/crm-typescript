# ComCrmPassSelfServiceResourceRedeemPassOrganisation

The Organisation at which the Pass was redeemed. If not specified, then the Pass is considered as redeemed at the business

## Example Usage

```typescript
import { ComCrmPassSelfServiceResourceRedeemPassOrganisation } from "crmcom/models/operations";

let value: ComCrmPassSelfServiceResourceRedeemPassOrganisation = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  merchantTap: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    code: "2131424123",
  },
  venueTap: {
    id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
    code: "2131424123",
  },
};
```

## Fields

| Field                                                                                                                                                   | Type                                                                                                                                                    | Required                                                                                                                                                | Description                                                                                                                                             | Example                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                    | *string*                                                                                                                                                | :heavy_minus_sign:                                                                                                                                      | The entity identifier that will be created                                                                                                              | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                    |
| `merchantTap`                                                                                                                                           | [operations.ComCrmPassSelfServiceResourceRedeemPassMerchantTap](../../models/operations/com-crm-pass-self-service-resource-redeem-pass-merchant-tap.md) | :heavy_minus_sign:                                                                                                                                      | The transaction acquiring point that the event was submitted from (id or code must be specified), usualy a unique number-based code                     |                                                                                                                                                         |
| `venueTap`                                                                                                                                              | [operations.ComCrmPassSelfServiceResourceRedeemPassVenueTap](../../models/operations/com-crm-pass-self-service-resource-redeem-pass-venue-tap.md)       | :heavy_minus_sign:                                                                                                                                      | The transaction acquiring point that the event was submitted from (id or code must be specified), usualy a unique number-based code                     |                                                                                                                                                         |