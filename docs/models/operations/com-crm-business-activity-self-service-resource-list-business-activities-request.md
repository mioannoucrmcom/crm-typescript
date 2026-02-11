# ComCrmBusinessActivitySelfServiceResourceListBusinessActivitiesRequest

## Example Usage

```typescript
import { ComCrmBusinessActivitySelfServiceResourceListBusinessActivitiesRequest } from "crmcom/models/operations";

let value:
  ComCrmBusinessActivitySelfServiceResourceListBusinessActivitiesRequest = {
    sort: "CREATED_DATE, UPDATED_DATE, NAMES, CHEDULED_DATE",
  };
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       | Example                                                                           |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `assignedToOrganisation`                                                          | *boolean*                                                                         | :heavy_minus_sign:                                                                | Defines whether to retrieve only business activities assigned to the organisation |                                                                                   |
| `name`                                                                            | *string*                                                                          | :heavy_minus_sign:                                                                | The name of the business activity                                                 |                                                                                   |
| `order`                                                                           | *string*                                                                          | :heavy_minus_sign:                                                                | Defines how the results will be ordered</br>Default:DESC                          |                                                                                   |
| `page`                                                                            | *number*                                                                          | :heavy_minus_sign:                                                                | The page number that should be retrieved</br>Default:1                            |                                                                                   |
| `size`                                                                            | *number*                                                                          | :heavy_minus_sign:                                                                | The size (total records) of each page</br>Default:10                              |                                                                                   |
| `sort`                                                                            | *string*                                                                          | :heavy_minus_sign:                                                                | Defines on which attribute the results should be sorted</br>Default:CREATED_DATE  | CREATED_DATE, UPDATED_DATE, NAMES, CHEDULED_DATE                                  |