# ComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchaseOrganisation

Details about the organisation that submitted such purchase

## Example Usage

```typescript
import { ComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchaseOrganisation } from "crmcom/models/operations";

let value:
  ComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchaseOrganisation = {
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

| Field                                                                                                                                                                                                 | Type                                                                                                                                                                                                  | Required                                                                                                                                                                                              | Description                                                                                                                                                                                           | Example                                                                                                                                                                                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                                                                                                  | *string*                                                                                                                                                                                              | :heavy_minus_sign:                                                                                                                                                                                    | The entity identifier that will be created                                                                                                                                                            | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                                                                                                                                                                  |
| `merchantTap`                                                                                                                                                                                         | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchaseMerchantTap](../../models/operations/com-crm-purchase-customer-event-self-service-resource-reclaim-purchase-merchant-tap.md) | :heavy_minus_sign:                                                                                                                                                                                    | The transaction acquiring point that the event was submitted from (id or code must be specified), usualy a unique number-based code                                                                   |                                                                                                                                                                                                       |
| `venueTap`                                                                                                                                                                                            | [operations.ComCrmPurchaseCustomerEventSelfServiceResourceReclaimPurchaseVenueTap](../../models/operations/com-crm-purchase-customer-event-self-service-resource-reclaim-purchase-venue-tap.md)       | :heavy_minus_sign:                                                                                                                                                                                    | The transaction acquiring point that the event was submitted from (id or code must be specified), usualy a unique number-based code                                                                   |                                                                                                                                                                                                       |