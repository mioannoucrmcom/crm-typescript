# ComCrmOrganisationSelfServiceResourceGetSingleOperationDetails

Defines the operation details of the organisation

## Example Usage

```typescript
import { ComCrmOrganisationSelfServiceResourceGetSingleOperationDetails } from "crmcom/models/operations";

let value: ComCrmOrganisationSelfServiceResourceGetSingleOperationDetails = {
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

| Field                                                                                                                                                                                  | Type                                                                                                                                                                                   | Required                                                                                                                                                                               | Description                                                                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `openingHours`                                                                                                                                                                         | [operations.ComCrmOrganisationSelfServiceResourceGetSingleOpeningHour](../../models/operations/com-crm-organisation-self-service-resource-get-single-opening-hour.md)[]                | :heavy_minus_sign:                                                                                                                                                                     | Details about the organisation’s working hours                                                                                                                                         |
| `shortTermOperations`                                                                                                                                                                  | [operations.ComCrmOrganisationSelfServiceResourceGetSingleShortTermOperation](../../models/operations/com-crm-organisation-self-service-resource-get-single-short-term-operation.md)[] | :heavy_minus_sign:                                                                                                                                                                     | Details about the organisation’s availability to offer its services                                                                                                                    |