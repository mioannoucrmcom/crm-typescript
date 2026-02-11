# ComCrmServiceRequestSelfServiceResourceListStage

The stage of the service request within the queue

## Example Usage

```typescript
import { ComCrmServiceRequestSelfServiceResourceListStage } from "crm/models/operations";

let value: ComCrmServiceRequestSelfServiceResourceListStage = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  name: "Response submitted",
  colour: "#FA89CB",
  order: 5,
};
```

## Fields

| Field                                       | Type                                        | Required                                    | Description                                 | Example                                     |
| ------------------------------------------- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------- | ------------------------------------------- |
| `id`                                        | *string*                                    | :heavy_minus_sign:                          | The entity identifier                       | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0        |
| `name`                                      | *string*                                    | :heavy_minus_sign:                          | The name of the current queue stage         | Response submitted                          |
| `colour`                                    | *string*                                    | :heavy_minus_sign:                          | The hex colour code associated to the stage | #FA89CB                                     |
| `order`                                     | *number*                                    | :heavy_minus_sign:                          | The order of this stage in the sequence     | 5                                           |