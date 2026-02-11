# DateT

The date that the meter reading was captured

## Example Usage

```typescript
import { DateT } from "crmcom/models/operations";

let value: DateT = {
  from: 1683547447,
  to: 1683547447,
};
```

## Fields

| Field                                                                                                    | Type                                                                                                     | Required                                                                                                 | Description                                                                                              | Example                                                                                                  |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `from`                                                                                                   | *number*                                                                                                 | :heavy_minus_sign:                                                                                       | The "from" date that the meter reading was captured                                                      | 1683547447                                                                                               |
| `to`                                                                                                     | *number*                                                                                                 | :heavy_minus_sign:                                                                                       | The "to" date up to which the meter reading was captured (applicable only if the date is based on range) | 1683547447                                                                                               |