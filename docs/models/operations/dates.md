# Dates

The date on which such reading was performed (if not specified, current date will be set)

## Example Usage

```typescript
import { Dates } from "crm/models/operations";

let value: Dates = {
  from: 1683547447,
  to: 1683547447,
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         | Example                                             |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `from`                                              | *number*                                            | :heavy_minus_sign:                                  | The "from" date that the meter reading was captured | 1683547447                                          |
| `to`                                                | *number*                                            | :heavy_minus_sign:                                  | The "to" date that the meter reading was captured   | 1683547447                                          |