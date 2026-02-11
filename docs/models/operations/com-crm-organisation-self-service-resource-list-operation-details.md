# ComCrmOrganisationSelfServiceResourceListOperationDetails

Defines the operation details of the organisation

## Example Usage

```typescript
import { ComCrmOrganisationSelfServiceResourceListOperationDetails } from "crmcom/models/operations";

let value: ComCrmOrganisationSelfServiceResourceListOperationDetails = {
  openingHours: [
    {
      dayOfWeek: "MONDAY",
      open: "09:00",
      close: "17:00",
      operation: "DELIVERY",
    },
  ],
  shortTermOperations: [
    {
      isClosed: false,
    },
  ],
};
```

## Fields

| Field                                                                                                                                                                       | Type                                                                                                                                                                        | Required                                                                                                                                                                    | Description                                                                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `openingHours`                                                                                                                                                              | [operations.ComCrmOrganisationSelfServiceResourceListOpeningHour](../../models/operations/com-crm-organisation-self-service-resource-list-opening-hour.md)[]                | :heavy_minus_sign:                                                                                                                                                          | Details about the organisation’s working hours                                                                                                                              |
| `shortTermOperations`                                                                                                                                                       | [operations.ComCrmOrganisationSelfServiceResourceListShortTermOperation](../../models/operations/com-crm-organisation-self-service-resource-list-short-term-operation.md)[] | :heavy_minus_sign:                                                                                                                                                          | Details about the organisation’s availability to offer its services                                                                                                         |