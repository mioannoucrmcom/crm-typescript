# ComCrmNameDayRulesSelfServiceResourceListNameDayRulesResponse

OK

## Example Usage

```typescript
import { ComCrmNameDayRulesSelfServiceResourceListNameDayRulesResponse } from "crmcom/models/operations";

let value: ComCrmNameDayRulesSelfServiceResourceListNameDayRulesResponse = {
  id: "4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0",
  names: "Marios, Maria",
  description: "Holly Mary",
};
```

## Fields

| Field                                                   | Type                                                    | Required                                                | Description                                             | Example                                                 |
| ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- |
| `id`                                                    | *string*                                                | :heavy_minus_sign:                                      | The entity identifier                                   | 4c01d5e4-02c9-ae89-4a3c-eaeb3174fcf0                    |
| `day`                                                   | *number*                                                | :heavy_minus_sign:                                      | The day of the name day                                 |                                                         |
| `month`                                                 | *number*                                                | :heavy_minus_sign:                                      | The month of the name day                               |                                                         |
| `names`                                                 | *string*                                                | :heavy_minus_sign:                                      | A comma separated list of names celebrating on this day | Marios, Maria                                           |
| `description`                                           | *string*                                                | :heavy_minus_sign:                                      | A description of the name day                           | Holly Mary                                              |