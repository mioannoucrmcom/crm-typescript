# ComCrmContactSelfServiceResourceAddContactRelationshipUsageAllowance

Defines the usage allowance

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceAddContactRelationshipUsageAllowance } from "crmcom/models/operations";

let value:
  ComCrmContactSelfServiceResourceAddContactRelationshipUsageAllowance = {
    organisations: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                                         | Type                                                                                                                                                                                                          | Required                                                                                                                                                                                                      | Description                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `accumulatedAllowance`                                                                                                                                                                                        | [operations.ComCrmContactSelfServiceResourceAddContactRelationshipAccumulatedAllowance](../../models/operations/com-crm-contact-self-service-resource-add-contact-relationship-accumulated-allowance.md)      | :heavy_minus_sign:                                                                                                                                                                                            | N/A                                                                                                                                                                                                           |
| `organisations`                                                                                                                                                                                               | [operations.ComCrmContactSelfServiceResourceAddContactRelationshipOrganisation](../../models/operations/com-crm-contact-self-service-resource-add-contact-relationship-organisation.md)[]                     | :heavy_minus_sign:                                                                                                                                                                                            | N/A                                                                                                                                                                                                           |
| `sameAsOwner`                                                                                                                                                                                                 | *boolean*                                                                                                                                                                                                     | :heavy_minus_sign:                                                                                                                                                                                            | When set to true, the member will have the same usage allowance per product as the owner’s termed/one-time service. Either same_as_owner OR accumulated_allowance and/or products_allowance can be specified. |