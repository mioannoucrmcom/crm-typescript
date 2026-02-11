# ComCrmContactSelfServiceResourceUpdateContactRelationshipUsageAllowance

Defines the usage allowance

## Example Usage

```typescript
import { ComCrmContactSelfServiceResourceUpdateContactRelationshipUsageAllowance } from "crm/models/operations";

let value:
  ComCrmContactSelfServiceResourceUpdateContactRelationshipUsageAllowance = {
    organisations: [
      {
        id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
      },
    ],
  };
```

## Fields

| Field                                                                                                                                                                                                          | Type                                                                                                                                                                                                           | Required                                                                                                                                                                                                       | Description                                                                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `accumulatedAllowance`                                                                                                                                                                                         | [operations.ComCrmContactSelfServiceResourceUpdateContactRelationshipAccumulatedAllowance](../../models/operations/com-crm-contact-self-service-resource-update-contact-relationship-accumulated-allowance.md) | :heavy_minus_sign:                                                                                                                                                                                             | N/A                                                                                                                                                                                                            |
| `organisations`                                                                                                                                                                                                | [operations.ComCrmContactSelfServiceResourceUpdateContactRelationshipOrganisation](../../models/operations/com-crm-contact-self-service-resource-update-contact-relationship-organisation.md)[]                | :heavy_minus_sign:                                                                                                                                                                                             | N/A                                                                                                                                                                                                            |
| `sameAsOwner`                                                                                                                                                                                                  | *boolean*                                                                                                                                                                                                      | :heavy_minus_sign:                                                                                                                                                                                             | When set to true, the member will have the same usage allowance per product as the owner’s termed/one-time service. Either same_as_owner OR accumulated_allowance and/or products_allowance can be specified.  |